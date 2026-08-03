# Bio in Situ — site novo

Site estático feito em Astro (astro.build), sem servidor/banco de dados.

## Rodar localmente

npm install
npm run dev

Abre em http://localhost:4321

## Gerar a versão de produção

npm run build
npm run preview

## Estrutura

- src/pages/index.astro — Home (pronta nesta etapa)
- src/components/ — Header, Footer, EpisodeCard
- src/layouts/Layout.astro — layout base (head, header, footer)
- src/styles/global.css — paleta de cores, tipografia e tokens do design
- src/data/posts.json — 259 posts (Podcast + Revista) extraídos do export do WordPress

## Deploy no Vercel

1. Suba esta pasta pro seu repositório no GitHub.
2. No Vercel: Add New Project -> selecione o repositório.
3. Framework preset: Astro (o Vercel detecta sozinho).
4. Build command: npm run build / Output: dist (padrão, não precisa mexer).
5. Deploy.

## Pendências conhecidas (não bloqueiam este teste)

- As imagens dos episódios ainda apontam pro site WordPress atual
  (biologiainsitu.com.br/wp-content/uploads/...). Funciona enquanto o site antigo
  existir, mas antes de desligar o WordPress precisamos migrar essas imagens pra
  dentro deste projeto.
- O favicon ainda é o padrão do Astro — troco pelo ícone da marca numa próxima etapa.
- Próximas páginas (Podcast, Revista, Equipe, Contato, Apoio) e o Decap CMS entram
  nas próximas entregas.
