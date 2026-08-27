# INK STUART — versão estática (HTML)

Esta pasta é o site completo já convertido em **HTML + CSS + JS + imagens**.
Não precisa de servidor nem de build: qualquer alojamento de ficheiros serve
(GitHub Pages, Netlify, Vercel, cPanel, etc.).

## O que está aqui

- `index.html` — página inicial
- `retratos/`, `realismo/`, `realismo/animais/`, `lettering/`,
  `fineline-outras/`, `cicatrizadas/`, `pequenos-detalhes/`, `momentos/`,
  `sobre/` — cada uma com o seu `index.html`
- `portfolio/` — todas as fotografias
- `__l5e/` — logótipo e vídeo do casamento
- `assets/` — CSS e JavaScript
- `sitemap.xml`, `robots.txt`, `404.html`, `.nojekyll`

## Publicar no GitHub Pages

1. Cria (ou usa) um repositório no GitHub.
2. Copia **o conteúdo desta pasta** para a raiz do repositório
   (o `index.html` tem de ficar na raiz, não dentro de `static-site/`).
3. No GitHub: **Settings → Pages → Source: Deploy from a branch**,
   branch `main`, pasta `/ (root)`.
4. Em poucos minutos o site fica online.
5. Para usar `inkstuart.com`: **Settings → Pages → Custom domain**.

O ficheiro `.nojekyll` já está incluído — é obrigatório, senão o GitHub Pages
ignora a pasta `assets/`.

## Testar no computador antes de publicar

```bash
cd static-site
python3 -m http.server 8000
```
Depois abre http://localhost:8000

## Atualizar no futuro

Sempre que fizermos alterações no projeto Lovable, é preciso voltar a gerar
esta pasta — os HTML aqui são uma "fotografia" do site nesse momento.

Nota: o vídeo do casamento foi comprimido (6,9 MB) para respeitar o limite de
100 MB por ficheiro do GitHub e carregar mais depressa.
