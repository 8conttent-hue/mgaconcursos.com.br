# CLAUDE.md — MGACONCURSOS

Site gerado pelo **SF (Site Factory)** em 15/04/2026.

## Contexto do Site

**Nome:** MGACONCURSOS
**Nicho:** Educação
**Keywords:** teacher Lugar certo de aprendizagem Aqui e o melhor lugar para voce
**Paleta de cores:** forest | **Fonte:** outfit

teacher Lugar certo de aprendizagem Aqui é o melhor lugar para você receber notícias, dicas e informações sobres o concurso que tanto deseja passar teacher2 Trabalhando com amor e eficiência Nossa equipe é composta por dezenas de professores que trabalham com paixão para entregar seu vasto conteúdo. teacher3 Mantenha-se sempre atualizado Mantenha-se sempre atualizado com as informações mais relevantes a cerca do concurso que tanto almeja.



## Componentes visuais usados

| Seção | Variante |
|-------|----------|
| Header | Header-F |
| Hero | Hero-F |
| Features | Features-I |
| About Section | About-I |
| Posts | Posts-D |
| Footer | Footer-D |
| Página Sobre | Sobre-F |
| Página Contato | Contato-F |

## Estrutura do projeto

```
src/
  sections/        # Layout escolhido pelo SF — Header, Hero, Features, About, Posts, Footer, Sobre, Contato
  data/            # JSONs com todo o conteúdo editável
  content/blog/    # Posts em Markdown
  pages/           # Rotas Astro (index, sobre, contato, blog, privacidade, termos)
  layouts/         # BaseLayout com fonte e cores dinâmicas
  styles/          # global.css com variáveis CSS de cor
public/
  images/          # hero.jpg, about.jpg, blog/*.jpg — inseridos automaticamente via Pexels
```

## O que editar

### Textos e conteúdo
- **`src/data/home.json`** — hero (título, subtítulo, botão), features (título, items), about section (título, desc, stats), posts
- **`src/data/sobre.json`** — conteúdo completo da página Sobre (hero, texto, missão)
- **`src/data/contato.json`** — título, subtítulo, email, tempo de resposta
- **`src/data/siteConfig.json`** — nome, slug, email, redes sociais, menu

### Imagens
Imagens já estão em `public/images/` (via Pexels). Para substituir, mantenha os mesmos nomes de arquivo:
- `hero.jpg` — imagem de fundo do Hero
- `about.jpg` — imagem da seção About (home)
- `sobre.jpg` — imagem de fundo da página Sobre
- `blog/{slug}.jpg` — imagens dos posts

### Posts do blog
Arquivos em `src/content/blog/`. Ajuste o tom de voz, adicione dados específicos do nicho e personalize conforme a identidade do site.

### Cores
Variáveis em `src/styles/global.css`: `--color-primary`, `--color-accent`, `--color-dark`.

## Deploy

```bash
bun install
bun run build
# Faça upload da pasta dist/ para Netlify, Vercel ou hosting estático
```
