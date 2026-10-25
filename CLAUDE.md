# apofenia7/apofenia7

Repositório de perfil do GitHub. Contém um `README.md` e as imagens em `assets/`.
Não é o spine (`~/APF`) nem um produto — não adicione build, CI, framework ou
documentação de arquitetura aqui.

## Invariantes

- **Nomes.** O card mostra a marca guarda-chuva, não o app. A marca pública de
  saúde é **Alternamente** (`alternamentesaude.com`). **Práxis** é o app clínico
  dentro dela, extraído para o repo `alternamente-praxis` em 18/07/2026 — não é
  marca descontinuada, é outra camada. Por isso o card diz Alternamente e não
  "Práxis Care": o visitante do perfil chega pela marca, não pelo app. No
  registro, Práxis aparece só como nome + estado, marcado "inside Alternamente".
- **Este repo não é fonte de verdade sobre o ecossistema.** Os protocolos
  transversais vivem em `claude-home-config/protocolos/`. Não replique doutrina
  aqui; linke ou nada.
- **Sem conteúdo de fachada.** Nenhum título, card ou seção sem destino ou texto
  real. Seção vazia sai da página; volta quando houver o que mostrar.
- **Links.** Todo projeto com destino público linka do próprio card. Os privados
  ficam sem link, cobertos pela nota "private repositories by design".

## Prancha e registro (desde 25/10/2026)

- O topo é a **Pl. 0 — le Fou**: a figura (silhueta do avatar no ar, asas de
  mariposa, a luz, o globo das capas le Fou Records) com a camada de anotação em
  magenta `#d4007a`. O texto público usa *le Fou* e "a figura do avatar, no ar",
  não "o louco" nem "a queda": o perfil linka a clínica, e essas palavras ao lado
  de apofenia leem como estigma ou romantização. Decisão de Mateus, 25/10/2026.
- **"The test"** é o registro dos sistemas na régua de 7 estados (proposed →
  generated → verified → integrated → deployed → observed → operable). Estado
  muda só com evidência e com data. Sistemas privados: nome + estado, sem link,
  sem descrição. Os estados de 25/10/2026 foram confirmados por Mateus.
- Para mudar um estado: troque `scale-N.svg` e o rótulo `N/7 · estágio` da
  linha, e atualize a data em "AS OF". Os `scale-1…7.svg` já existem.
- le Fou Records é selo **em preparação**: não escrever que está lançado.

## Imagens

- `assets/plate0/pl0-{light,dark}.svg`: prancha 880×628 com fundo opaco
  (`#ffffff` / `#0d1117`), para continuar legível quando o tema do GitHub
  diverge do tema do sistema. Figura embutida como PNG de paleta (960 px,
  6 níveis); textos convertidos em contorno (sem fontes externas).
- `scale-*.svg` e `tile-*.svg`: neutros (cinza `#6e7781` + magenta), um arquivo
  para os dois temas.
- Capas `lefou-*.jpg`: 440 px, JPEG progressivo, `quality=82`, `optimize=True`.
- Todo `<img>` precisa de `alt` descritivo — descreve a imagem, não o projeto.
- Peso: uma visita baixa ~500 KB (uma variante da prancha + capas + glifos).
  `assets/plate0/` soma ~715 KB. Os 7 JPGs do layout anterior (`assets/*.jpg`,
  ~410 KB) estão sem uso desde 25/10/2026; remover só com OK do Mateus.

## Layout

O registro usa `<table>` porque é o que o GitHub renderiza. Em mobile a tabela
vira scroll horizontal — limitação conhecida e aceita. Não troque por outro
esquema sem testar no app do GitHub. `<picture>` com `prefers-color-scheme`
escolhe a prancha clara ou escura; escreva `<picture>`/`<source>` numa linha só.

## Pendência conhecida

O link "website" aponta para `mateusabreu.vercel.app` (destino do antigo
`mateus-site-ebon.vercel.app`) — ainda subdomínio autogerado ao lado de dois
domínios próprios. Substituir por domínio próprio.
