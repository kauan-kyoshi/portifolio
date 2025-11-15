# Portfólio 42SP (Astro)

Site estático para apresentar projetos da 42SP e pessoais.

## Tecnologias
- Astro
- Tailwind CSS

## Comandos
```bash
npm install
npm run dev
```

Build de produção:
```bash
npm run build
npm run preview
```

## Estrutura
- `src/pages`: páginas (`/`, `/projects`, `/about`)
- `src/components`: componentes reutilizáveis
- `src/layouts`: layout base
- `src/data/projects.json`: dados dos projetos (edite com seus links)

## Personalização rápida
- Atualize `src/data/projects.json` com seus repositórios e tags.
- Troque email e descrição em `src/pages/about.astro`.
- Ajuste cores em `tailwind.config.mjs`.

## Deploy
- Qualquer host estático (Vercel, Netlify, GitHub Pages).
- Em Vercel, framework = Astro; comando build `npm run build`; diretório `.astro` gera `dist/`.