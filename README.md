# ! Projeto Portal de Animes — Plataforma Interativa e Gamificada
## " Visão Geral
Um site moderno, interativo e gamificado dedicado a informações sobre animes,
com foco em **experiência de usuário**, **personalização** e **integração com
APIs**.
O objetivo é criar uma alternativa mais dinâmica e visualmente atraente que sites
tradicionais como MyAnimeList ou AniList.
> “Um portal de animes moderno, com informações da temporada, contagem de
episódios, gamificação e personalização — tudo com foco em design, fluidez e
recompensas pela interação.”
---
## # Funcionalidades Principais
| Categoria | Descrição |
|------------|------------|
| $ **Animes da temporada** | Exibe todos os animes em exibição com contagem
regressiva para o próximo episódio. |
| ⏳ **Contagem dinâmica** | Cada anime mostra quanto tempo falta até o novo
episódio. Após o lançamento, o card se reposiciona automaticamente. |
| & **Comentários e Spoilers** | Área de comentários com uma sub-seção exclusiva
para spoilers (marcada visualmente). |
| ' **Gamificação** | Usuários ganham pontos ao comentar, reagir, ler notícias e
interagir no site. |
| ( **Sistema de pontos** | Pontos podem ser trocados por benefícios: <br>•
Remover anúncios <br>• Personalizar o tema do site <br>• Desbloquear funções
extras |
| ) **Temas personalizados** | Tema claro/escuro base e temas adicionais
desbloqueáveis (ex: azul, roxo, verde, etc). |
| * **Integração com streaming** | Links diretos para assistir em plataformas
oficiais (Crunchyroll, Netflix, etc). |
| + **Relacionamento entre temporadas e filmes** | Mostra se há filmes, OVAs ou
novas temporadas relacionadas. |
| $ **Área de Notícias** | Notícias gerais sobre o mundo dos animes e atualizações
específicas em cada página de anime. |
---
## $ Área de Notícias
### Estrutura de conteúdo
1. **Página geral de notícias (`/noticias`)**
 - Destaque principal (notícia mais recente ou popular).
 - Cards em grade com miniaturas e resumos.
 - Filtros por anime, data e tipo (ex: *Anúncio*, *Trailer*, *Evento*).
2. **Página individual (`/noticia/id`)**
 - Título, imagem principal, corpo do texto.
 - Data, fonte e tags de categoria.
 - Reações e comentários de usuários.
 - Notícias relacionadas no final.
3. **Integração com a página do anime (`/anime/nome`)**
 - Aba **“Notícias”** dentro da página do anime.
 - Mostra apenas as notícias relacionadas.
 - Permite comentários e geração de pontos.
### Exemplo de estrutura JSON
```json
[
 {
 "id": 1,
 "titulo": "Attack on Titan 4ª temporada confirmada!",
 "anime": "Attack on Titan",
 "data": "2025-11-02",
 "categoria": "Anúncio",
 "imagem": "aot4.jpg",
 "conteudo": "O estúdio MAPPA confirmou...",
 "fonte": "Crunchyroll News"
 }
]
```
### Pontos por interação
| Ação | Pontos |
|------|--------|
| Ler uma notícia até o fim | +1 |
| Comentar na notícia | +2 |
| Reagir (like/hype) | +0.5 |
| Publicar uma notícia aprovada | +5 |
---
## ! Design e Interface
**Estilo:** moderno, limpo, inspirado em streaming (Netflix / Crunchyroll).
**Paleta:** tons neutros + cor de destaque (ex: laranja ou roxo).
**Temas:** claro, escuro e temas desbloqueáveis por pontos.
**Layout principal:**
```
HEADER → logo | busca | menu | botão de tema
MAIN → seção de temporada | lançamentos | notícias
FOOTER → créditos e APIs
```
---
## ! Etapas Técnicas
| Etapa | Descrição | Status |
|--------|------------|--------|
| **1. Estrutura HTML** | Criar a estrutura de todas as seções (home, notícias, página
do anime). | " |
| **2. Estilização CSS** | Implementar layout responsivo e temas claro/escuro com
variáveis CSS. | " |
| **3. Interatividade JS** | Alternância de tema, contagem regressiva e manipulação
básica de cards. | # |
| **4. Consumo de API AniList** | Obter dados reais dos animes da temporada. | # |
| **5. Sistema de gamificação (back-end)** | Login, pontos e personalização por
usuário. | # |
| **6. Publicação (GitHub Pages)** | Tornar o protótipo acessível online. | # |
---
## $ Plano de Aprendizado
### Fase 1 — Front-end
- Reforçar **HTML semântico**, **CSS Grid/Flexbox** e **variáveis CSS**.
- Aprender **JavaScript DOM e temporizadores**.
- Introdução a **APIs REST** com `fetch()`.
### Fase 2 — Back-end
- Aprender **Python (Flask/FastAPI)** ou **Node.js (Express)**.
- Criar banco de dados simples (**SQLite** ou **MongoDB**).
- Implementar login e persistência de pontos.
### Fase 3 — Projeto Completo
- Adicionar autenticação real, rankings e personalização de temas.
- Otimizar design, desempenho e SEO.
---
## ! Estrutura de Pastas Sugerida
```
anime-portal/
│
├── docs/
│ ├── roadmap.md
│ ├── funcionalidades.md
│ └── design-wireframes/
│
├── src/
│ ├── index.html
│ ├── style.css
│ └── script.js
│
└── README.md
```
---
## " Próximos Passos
1. Criar o repositório `anime-portal-prototype` no GitHub.
2. Adicionar este README.md.
3. Criar o layout base em HTML/CSS com suporte a tema claro/escuro.
4. Adicionar a área de notícias.
5. Publicar no GitHub Pages e testar responsividade.
---
**Autor:** [Erick Silva](https://github.com/Erick-SL)
**Mentoria e estruturação:** ChatGPT (GPT-5)
# *Início do projeto:* Novembro de 2025
