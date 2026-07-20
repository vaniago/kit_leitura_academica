---
name: triagem-de-leitura
description: >
  Use esta skill quando a pessoa tiver um texto para estudar mas não
  souber qual skill de leitura deste kit é a mais adequada, ou pedir
  explicitamente ajuda para escolher entre elas. Gatilhos: "não sei qual
  skill de leitura usar", "qual desses métodos serve pro meu caso",
  "tenho um texto mas não sei por onde começar", "quero ler isso mas não
  sei qual abordagem usar", "me ajuda a escolher a skill certa pra esse
  texto", "quais skills de leitura vocês têm", "qual a diferença entre as
  skills de leitura". NÃO use esta skill se a pessoa já indicou o método,
  o tipo de texto ou a skill desejada de forma clara (ex.: "quero um
  fichamento", "quero aplicar o método das três passadas nesse paper",
  "quero estudar esse poema com o Cosson", "só tenho o livro físico, sem
  digitalização") — nesses casos, vá direto para a skill específica
  correspondente.
---

# Triagem de Leitura

Esta skill não conduz uma sessão de leitura — ela existe só para ajudar a
pessoa a escolher, entre as demais skills deste kit, qual encaixa melhor
com o texto e o objetivo dela. Depois de recomendar, encerre esta skill e
siga para a skill recomendada (se ela estiver disponível) ou oriente a
instalação.

## Princípios gerais

- **Uma pergunta de cada vez.** Nunca liste as seis skills de uma vez
  esperando que a pessoa escolha sozinha por um menu — conduza uma
  triagem breve, pergunta a pergunta, do mesmo jeito que as demais skills
  do kit conduzem suas entrevistas.
- **Recomende, não decida por decisão vaga.** Se a resposta da pessoa for
  ambígua o bastante para caber em mais de uma skill, diga isso
  abertamente, explique a diferença em uma frase por opção, e deixe a
  escolha final com a pessoa.
- **Não repita o README linha a linha.** As explicações abaixo servem de
  apoio interno para a triagem — na conversa, resuma em frases curtas,
  sem ler os parágrafos deste arquivo em voz alta.
- **Tom casualmente polido**, mesmo cuidado das demais skills do kit.
- **Linguagem neutra**, sem declinar gênero, a menos que a pessoa
  sinalize a forma preferida.

## Fluxo de triagem

### 1. Tipo de texto
Pergunte, numa frase: que tipo de texto é — um artigo científico, uma
obra literária (poema, conto, romance, crônica, peça), um capítulo de
livro didático que só existe em papel, ou outro texto acadêmico/técnico
(artigo, capítulo, resumo) já digitalizado (colado, anexado ou por
link)?

Direcione pela resposta:
- **Artigo científico único** (não é comparação entre vários artigos) →
  recomende `leitura-cientifica-keshav`. Vá para o passo 3.
- **Obra literária** → recomende `leitura-literaria-cosson`. Vá para o
  passo 3.
- **Capítulo de livro didático impresso, sem versão digital** →
  recomende `leitura-livro-didatico-sem-digitalizacao`. Vá para o passo 3.
- **Outro texto acadêmico/técnico digitalizado** → vá para o passo 2
  antes de recomendar.

Se a pessoa mencionar comparação entre vários artigos ou fontes (revisão
de literatura), diga com clareza que nenhuma skill deste kit cobre isso
hoje — todas tratam de um texto ou uma obra por vez — e não force um
encaixe forçado em nenhuma delas.

### 2. Objetivo (só para texto acadêmico/técnico genérico)
Pergunte, numa frase, o que a pessoa mais precisa deste momento de
leitura:
- **Um documento de análise formal para consultar depois** (fichamento,
  resenha, resumo indicativo/informativo, registro de citações) →
  recomende `leitura-analitica-severino`.
- **Ter certeza de que realmente entendeu o núcleo do texto**, com
  checagem constante de compreensão, mesmo que isso signifique
  reorganizar a ordem do conteúdo → recomende `tutor-de-texto`.
- **Ser acompanhada na leitura na própria ordem em que o texto se
  desenrola**, sem um método de análise formal nem reorganização
  pedagógica, com apoio ao contexto e ao que já sabe → recomende
  `leitura-guiada`.

Se a resposta ficar entre duas dessas opções (é comum entre
`tutor-de-texto` e `leitura-guiada`, ou entre `tutor-de-texto` e
`leitura-analitica-severino`), explique a diferença central em uma frase
por opção e pergunte qual pesa mais para a pessoa agora.

**Se a pessoa não souber responder** — sinais como "não sei", "tô muito
perdida nesse texto", "não faço ideia do que preciso", ou qualquer
resposta que mostre insegurança com o próprio texto, não com a escolha
entre skills — não force uma decisão entre as três opções. Explique, em
poucas frases, que isso costuma indicar que o texto ainda não tem uma
base de compreensão clara, mais do que indecisão sobre qual skill usar,
e que o caminho mais seguro nesse caso costuma ser começar por
`tutor-de-texto` (que verifica a compreensão passo a passo e não exige
que a pessoa já saiba o que precisa) ou por `leitura-guiada` (que também
não exige um objetivo definido de antemão, só acompanha o texto na
própria ordem em que ele vem) — deixando o documento formal do
`leitura-analitica-severino`, ou uma leitura mais crítica, para depois,
quando o texto já estiver mais claro. Ainda assim, apresente isso como
explicação, não como decisão pronta: a escolha final continua com a
pessoa.

### 3. Confirmação e encaminhamento
Apresente a recomendação com uma justificativa breve (1-2 frases: por que
essa skill e não outra, dado o que a pessoa respondeu) e pergunte se quer
seguir com ela.

- Se a pessoa confirmar e a skill recomendada estiver disponível no
  ambiente atual, siga diretamente as instruções dela a partir daqui,
  sem reabrir a triagem.
- Se a skill recomendada **não** estiver instalada, diga isso com
  clareza, informe o nome exato da pasta/skill e oriente a instalação a
  partir do [README do kit](../README.md) — nunca tente simular o
  comportamento da outra skill de memória.
- Se a pessoa preferir ver as outras opções antes de decidir, descreva
  em uma frase cada skill ainda não mencionada, sem entrar em detalhes de
  fluxo interno.

## Cuidados

- Não conduza nenhum trecho de leitura, análise ou fichamento dentro
  desta skill — o papel dela é só recomendar e encaminhar.
- Não invente uma sétima abordagem por conta própria para tentar encaixar
  um caso que não se encaixa bem em nenhuma das seis — nesse caso, diga
  isso abertamente à pessoa.
- Se, no meio da triagem, a pessoa já disser claramente qual skill quer
  (ex.: "ah, então quero o fichamento mesmo"), pule direto para o
  encaminhamento, sem insistir nas perguntas restantes.
