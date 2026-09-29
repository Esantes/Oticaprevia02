# Landing page — Ótica Íris (modelo)

Abra o `index.html` direto no navegador. Não precisa de servidor nem de instalação.

## Estrutura

```
index.html          estrutura e textos
css/style.css       visual (cores e fontes no bloco :root, no topo)
js/script.js        dados da loja, vitrine, menu, WhatsApp, animações
images/             favicon, imagem reserva e pastas para as fotos reais
```

## Checklist antes de publicar

**1. Dados da loja — `js/script.js`, objeto `CONFIG`**
Número do WhatsApp (só dígitos, `55` + DDD + número), telefone, Instagram, endereço, horário e o texto de busca do mapa. Esses dados são aplicados automaticamente no header, contato, rodapé, mapa e botão "Como chegar".
Se o número continuar o de exemplo, o console do navegador (F12) mostra um aviso.

**2. Textos que também estão no HTML (por causa do Google)**
Procure e troque em `index.html`: `Ótica Íris`, `oticairis.com.br`, `Rua Exemplo`, `3000-0000`, `99999-9999`.
Ficam no `<title>`, na meta description, no Open Graph, no bloco JSON-LD (dados estruturados) e no horário do contato/rodapé.

**3. Vitrine — `js/script.js`, lista `PRODUTOS`**
Cada item tem nome, rótulo, categorias, descrição, imagem e alt. Para adicionar um modelo, copie um bloco e edite. Categorias válidas: `grau`, `sol`, `masculino`, `feminino`, `infantil`.

**4. Fotos**
As fotos atuais são demonstrativas (Unsplash, uso comercial permitido). Troque pelas fotos reais:
- salve em `images/products/`, `images/banners/` etc.;
- prefira WebP, com lado maior entre 1200 e 1600 px (dá para converter em squoosh.app);
- na vitrine, troque `imagem: unsplash('...')` por `imagem: 'images/products/aurora.webp'`;
- no HTML, troque o `src` (e apague o `srcset` do hero, ou gere as versões 640/1000/1600).
A categoria **Infantil** está sem foto de criança: é a primeira a trocar.
Se alguma imagem falhar, o site mostra `images/placeholder.svg` no lugar.

**5. Marcas** — só liste marcas que a loja realmente revende. Para usar logos, peça os arquivos oficiais ao fornecedor e coloque um `<img>` dentro de cada `<li>`.

**6. Depoimentos** — os três são provisórios. Substitua por avaliações reais (Google, por exemplo), com autorização do cliente. Depoimento inventado em site comercial é propaganda enganosa.

**7. Cores e fontes** — bloco `:root` no topo do `style.css`.
