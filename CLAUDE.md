# apofenia7/apofenia7

Repositório de perfil do GitHub. Contém um `README.md` e as imagens em `assets/`.
Não é o spine (`~/APF`) nem um produto — não adicione build, CI, framework ou
documentação de arquitetura aqui.

## Invariantes

- **Nomes.** O card mostra a marca guarda-chuva, não o app. A marca pública de
  saúde é **Alternamente** (`alternamentesaude.com`). **Práxis** é o app clínico
  dentro dela, extraído para o repo `alternamente-praxis` em 18/07/2026 — não é
  marca descontinuada, é outra camada. Por isso o card diz Alternamente e não
  "Práxis Care": o visitante do perfil chega pela marca, não pelo app.
- **Este repo não é fonte de verdade sobre o ecossistema.** Os protocolos
  transversais vivem em `claude-home-config/protocolos/`. Não replique doutrina
  aqui; linke ou nada.
- **Sem conteúdo de fachada.** Nenhum título, card ou seção sem destino ou texto
  real. Seção vazia sai da página; volta quando houver o que mostrar.
- **Links.** Todo projeto com destino público linka do próprio card. Os privados
  ficam sem link, cobertos pela nota "private repositories by design".

## Imagens

- Cards renderizam a ~300px em grid de 3 colunas: exporte a **800px** de largura.
- Hero renderiza full-width: exporte a **1800px**.
- JPEG progressivo, `quality=82`, `optimize=True`. Alvo: `assets/` abaixo de 500 KB
  no total (hoje: ~410 KB). Não commite export de 1536px direto do gerador.
- Todo `<img>` precisa de `alt` descritivo — os atuais descrevem a imagem, não o
  projeto; mantenha esse padrão.

## Layout

O grid usa `<table>` porque é o que o GitHub renderiza. Em mobile a tabela vira
scroll horizontal — limitação conhecida e aceita. Não troque por outro esquema
sem testar no app do GitHub.

## Pendência conhecida

O primeiro link do header aponta para `mateus-site-ebon.vercel.app` — subdomínio
autogerado ao lado de dois domínios próprios. Substituir por domínio próprio.
