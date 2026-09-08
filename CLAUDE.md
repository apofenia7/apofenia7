# apofenia7/apofenia7

Repositório de perfil do GitHub. Contém um `README.md` e as imagens em `assets/`.
Não é o spine (`~/APF`) nem um produto — não adicione build, CI, framework ou
documentação de arquitetura aqui.

## Invariantes

- **Nomes.** O produto de saúde chama-se **Alternamente** (`alternamentesaude.com`).
  "Práxis Care" foi descontinuado como nome público. Um projeto tem um nome só,
  e ele aparece igual no card e no link.
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
