---
name: leitura-analitica-severino
description: >
  Use esta skill sempre que o usuário pedir um "fichamento", "leitura analítica",
  "ficha de leitura", "resumo crítico de texto acadêmico", "análise de texto"
  filosófico/científico, ou pedir ajuda para estudar, resumir ou tirar notas
  estruturadas de um texto acadêmico — mesmo que não mencione "Severino" ou
  "fichamento" explicitamente (ex.: "resume esse capítulo de forma acadêmica",
  "preciso estudar esse texto pra prova", "quero fazer uma leitura analítica
  desse texto"). A skill aplica o método de leitura analítica de Antônio Joaquim
  Severino (Metodologia do Trabalho Científico) e sempre entrega o resultado
  como um arquivo markdown (.md) pronto para download. Diferente de
  tutor-de-texto (sessão interativa que reorganiza o conteúdo numa sequência
  pedagógica própria) e de leitura-guiada (acompanhamento sequencial do texto,
  centrado no leitor, sem aplicar um método formal de análise): esta skill
  entrega um documento de análise estruturado. Se o pedido for só "me ajuda a
  entender esse artigo" ou "me acompanha na leitura", sem indicar que o
  usuário quer um documento de análise formal, considere tutor-de-texto ou
  leitura-guiada antes de aplicar esta skill.
---

# Leitura Analítica e Fichamento — Método Severino

Esta skill guia a leitura analítica de um texto acadêmico e a produção de um
fichamento, seguindo o roteiro proposto por Antônio Joaquim Severino em
*Metodologia do Trabalho Científico*. O processo interno é sempre o mesmo
(as cinco etapas abaixo); o que muda é o **formato de saída**, que o usuário
escolhe.

**Referência bibliográfica do método (ABNT):**
SEVERINO, Antônio Joaquim. *Metodologia do trabalho científico*. 24. ed.
rev. e ampl. São Paulo: Cortez, 2017.

## Fluxo de trabalho

1. **Obtenha o texto.** Se o usuário não colou ou anexou o texto, peça que
   envie (cole o trecho, anexe um PDF/DOCX ou indique o link). Não invente
   conteúdo de um texto que não foi fornecido. Se o texto não estiver em
   português, pergunte o nível de compreensão do usuário no idioma original
   (nada, muito pouco, pouco, razoável, bom, ótimo) e ajuste a densidade das
   paráfrases no fichamento a esse nível — nunca produza uma tradução
   completa do texto (ver "Cuidados").
2. **Delimite a unidade de leitura.** Se o texto for longo (mais que um
   capítulo curto), pergunte se o usuário quer fichar o texto inteiro ou uma
   unidade específica (um capítulo, uma seção, um conjunto de parágrafos).
   Um fichamento por unidades menores tende a ser mais fiel ao método.
3. **Pergunte o formato de saída desejado** (se o usuário não tiver
   especificado), oferecendo as opções da seção "Tipos de fichamento"
   abaixo. Na dúvida ou se o usuário pedir "um fichamento" sem mais detalhes,
   use o **fichamento analítico integral** como padrão.
4. **Pergunte se o usuário também quer um mapa conceitual** (arquivo .txt
   no formato de importação do CmapTools) como entregável extra — ver seção
   "Mapa conceitual (formato CmapTools)" abaixo. É opcional e independente
   do tipo de fichamento escolhido.
5. **Se o formato escolhido for resenha completa (e) ou analítico integral
   (f)**, pergunte também qual **modo de condução** o usuário prefere para
   as etapas 3, 4 e 5 — diálogo, sugestões no documento ou método direto —
   ver seção "Modo de condução das etapas 3, 4 e 5" abaixo. O documento
   final é sempre o documento completo com as cinco etapas, independente do
   modo escolhido. Os demais formatos (bibliográfico, citações, resumo
   indicativo, resumo informativo) pulam essa pergunta.
6. **Execute as etapas 1 e 2 (textual e temática) sempre internamente**,
   independentemente do formato de saída — são a base de compreensão do
   texto que sustenta qualquer formato.
7. **Conduza as etapas 3, 4 e 5 conforme o modo escolhido** no passo 5,
   quando aplicável.
8. **Gere o arquivo .md** no formato escolhido, incorporando o que foi
   produzido em todas as etapas conduzidas.
9. **Se solicitado, gere também o arquivo .txt do mapa conceitual**, como
   arquivo separado do .md.
10. **Entregue sempre como arquivo(s) para download** (nunca só como texto
    na conversa) — use as ferramentas de criação de arquivo e disponibilize
    o(s) arquivo(s) gerado(s).

## As cinco etapas da leitura analítica

### 1. Análise textual
Primeiro contato com o texto: uma leitura atenta, mas ainda corrida, sem
buscar esgotar a compreensão. Nesta etapa, levante e registre:
- **Dados sobre o autor** (formação, época, escola de pensamento, obra em
  que o texto se insere).
- **Vocabulário e conceitos-chave** que precisam de esclarecimento para a
  compreensão do texto. Esteja atento ao vocabulário técnico e específico
  da área de conhecimento do texto e considere que o leitor é sempre um
  iniciante no tema.
- **Referências** a fatos históricos, outros autores ou doutrinas
  mencionados que exigem contextualização.

**Técnica auxiliar para textos longos ou muito técnicos:** quando útil,
monte um glossário dos termos técnicos ou menos comuns do texto (formato
`termo; significado conciso`, pelo menos vinte termos se o texto permitir)
e uma lista da ideia central de cada parágrafo (formato `número; ideia
central em texto conciso`). Como modelos de linguagem costumam errar a
contagem de parágrafos, se o usuário souber o total aproximado, peça essa
informação antes de gerar a lista (ex.: "considere que o texto tem
aproximadamente 50 parágrafos"). Inclua esses materiais como anexo do
fichamento quando forem produzidos.

### 2. Análise temática
Busca entender **do que o texto trata e o que o autor afirma**, portanto registre:
- Tema central da unidade de leitura.
- Problema que o autor está respondendo.
- Tese defendida.
- Argumentos principais: aqueles que demonstram diretamente que a tese é
  verdadeira.
- Argumentos secundários: aqueles que ajudam a compreender o problema, a
  solução, e explicam os argumentos principais, mas que poderiam não estar
  no texto.
- Conclusão a que o autor chega.

As etapas 3, 4 e 5 abaixo dependem do **modo de condução** escolhido pelo
usuário (ver seção específica mais adiante) — o conteúdo pode vir de uma
entrevista com o usuário ou ser apresentado como sugestões para o próprio
usuário desenvolver.

### 3. Análise interpretativa
Vai além do que está explícito no texto — é a chamada **crítica externa**:
o texto avaliado a partir de fora dele mesmo. Devem ser registrados:
- Pressupostos teóricos e filosóficos que o autor assume: princípios que
  podemos inferir do texto, mas que não estão explicitados.
- Com que hipóteses ou doutrinas o autor se identifica, e a quais se
  contrapõe.
- Em que debate ou tradição de pensamento o texto se situa (história das
  ideias/da área de pesquisa em questão).
- Comparação com posições afins ou opostas de outros autores/correntes
  (quando pertinente e sem inventar atribuições).

### 4. Problematização
Levantamento de questionamentos próprios sobre o texto, devem ser registrados:
- Pontos que ficaram em aberto, lacunas ou tensões internas.
- Perguntas que o texto suscita e que mereceriam mais discussão.
- Que novos problemas de pesquisa a leitura desse texto faz perceber.
- Não confundir com a "determinação do problema" da etapa 2 — aqui o
  questionamento é do leitor sobre o texto, não do autor sobre o mundo.

### 5. Síntese pessoal
Fechamento crítico do processo. A avaliação de coerência interna é a
**crítica interna**: o texto avaliado por seus próprios critérios. Devem
ser registrados:
- **Coerência interna** (crítica interna), com perguntas concretas:
  - O problema da unidade foi bem formulado, ou há falhas na formulação?
  - A tese apresentada é, de fato, uma solução para o problema proposto?
  - Os argumentos demonstram a solução defendida?
  - Os argumentos são válidos e as informações apresentadas são
    verdadeiras ou, no mínimo, verificáveis?
- **Originalidade e contribuição**: o texto traz algo além da retomada de
  ideias de outros autores?
- **Posição pessoal do leitor** diante do que foi lido.

## Modo de condução das etapas 3, 4 e 5

As etapas de análise interpretativa, problematização e síntese pessoal
dependem do posicionamento do próprio leitor — não são algo que o Claude
deva simplesmente inventar em nome do usuário. Quando o formato de saída
for resenha completa (e) ou analítico integral (f), pergunte ao usuário
qual dos três modos prefere. Em qualquer um dos três, **o documento final
entregue é sempre o documento completo, com as cinco etapas** — o que muda
entre os modos é apenas como o conteúdo das etapas 3, 4 e 5 é obtido, nunca
a estrutura do arquivo final.

### Modo 1 — Diálogo (entrevista)
O Claude conduz uma conversa com o usuário para ajudá-lo a construir sua
própria análise, apoiando com sugestões — mas registrando no fichamento a
posição elaborada pelo usuário, não uma posição fabricada pelo Claude.
Nessa conversa, o Claude pode:
- sugerir possíveis pressupostos teóricos do autor para o usuário avaliar;
- apontar o estado da arte do debate externo ao texto (outras posições na
  literatura sobre o tema, pesquisando quando necessário);
- sugerir autores ou correntes para comparação;
- propor questionamentos que poderiam alimentar a problematização;
- apontar possíveis "furos" ou tensões na coerência interna do argumento,
  para o usuário confirmar, refutar ou completar;
- levantar pontos de originalidade a considerar;
- sugerir itens/eixos para o posicionamento pessoal do leitor (concordância,
  discordância, aplicação prática, limites do argumento, etc.).
O fichamento final registra as respostas e escolhas do usuário, não as
sugestões do Claude tomadas como se fossem a opinião dele.

### Modo 2 — Sugestões no documento
Em vez de dialogar, o Claude conclui sozinho as etapas 1 e 2 (textual e
temática) e, no próprio arquivo .md, lista as sugestões que orientariam a
sequência reflexiva das etapas 3, 4 e 5 — nos mesmos eixos do Modo 1
(pressupostos, estado da arte, autores para comparação, questionamentos,
possíveis furos na coerência interna, pontos de originalidade, sugestões de
posicionamento pessoal) — deixando claro que são sugestões de orientação, e
não a análise pronta, para o usuário desenvolver por conta própria depois.

### Modo 3 — Método direto (especialista)
O caminho mais rápido: sem diálogo, o Claude atua como especialista no
texto e preenche diretamente as etapas 3, 4 e 5 com sua própria leitura
especializada, respondendo objetivamente a perguntas como: que teorias e
doutrinas o autor segue; a que debate o texto se filia; com que obras
semelhantes pode ser comparado; qual o nível de dificuldade de leitura;
a que tipo de leitor o texto se dirige; e a avaliação de coerência interna
(as quatro perguntas da etapa 5). Deixe explícito no documento que esse
conteúdo é a leitura especializada do Claude, não a posição pessoal do
leitor — e mantenha em aberto o campo "posição pessoal do leitor" da etapa
5 para o usuário preencher depois, já que esse item não pode ser suprido
por uma leitura especializada externa.

Se o usuário não indicar preferência, pergunte diretamente; não presuma um
modo por padrão, já que mudam bastante o resultado final.

### Seção "Orientações para resenha/resumo crítico" — sempre presente

Independentemente do modo escolhido, o arquivo .md final de uma resenha
completa ou de um fichamento analítico integral deve manter uma seção
própria chamada **"Orientações para resenha/resumo crítico"**, com as
sugestões nos eixos listados acima (pressupostos, estado da arte do debate,
autores para comparação, questionamentos, possíveis furos na coerência
interna, pontos de originalidade, eixos de posicionamento pessoal).


- **No Modo 1 (diálogo):** essa seção registra as sugestões que o Claude
  ofereceu durante a conversa, como referência — mantida junto (não em
  lugar) da posição final que o usuário efetivamente construiu nas etapas
  3, 4 e 5.
- **No Modo 2 (sugestões no documento):** essa seção é o próprio conteúdo
  gerado pelo Claude, com espaço logo abaixo de cada item para o usuário
  preencher depois com sua posição.

Essa seção nunca substitui as etapas 3, 4 e 5 do template — ela é
complementar, um registro do apoio oferecido ao leitor.

## Tipos de fichamento (formatos de saída)

Ofereça estas opções ao usuário quando o formato não estiver claro:

### a) Fichamento bibliográfico
Registro enxuto: referência completa (ABNT), tema/objetivo da obra e
estrutura geral (capítulos/seções). Bom para catalogar um texto rapidamente.

### b) Fichamento de citações (transcrição)
Trechos literais mais relevantes do texto, cada um com a página de origem,
organizados na ordem em que aparecem. Use aspas e nunca reproduza passagens
muito longas — no máximo frases curtas por trecho selecionado.

### c) Resumo indicativo (NBR 6028)
Destaca apenas os pontos principais do texto (assunto, problema e tese),
se possível em um único parágrafo, sem apresentar dados qualitativos ou
quantitativos nem resultados detalhados. Não dispensa a consulta ao texto
original — serve para o leitor decidir se vale a pena lê-lo na íntegra.
Baseia-se nas etapas 1 e 2.

### d) Resumo informativo (NBR 6028)
Mais completo que o indicativo: em até 500 palavras, apresenta finalidade,
metodologia (quando aplicável), resultados e conclusões do texto, de forma
que possa, em algum grau, dispensar a consulta ao original. Ainda assim,
sem opinião do leitor e sem citações diretas. Baseia-se nas etapas 1 e 2.

### e) Resenha completa / Resumo crítico (NBR 6028)
Resumo do conteúdo **mais** avaliação crítica do leitor — equivale, na
prática, a apresentar as etapas 2, 3 e 5 de forma corrida e em prosa. Por
depender da manifestação do leitor (etapas 3 a 5), só deve ser produzido
depois de conduzir o modo de condução escolhido (ver seção acima) — não é
possível gerar um resumo crítico legítimo sem essa etapa de posicionamento.

### f) Fichamento analítico integral (padrão)
Apresenta as cinco etapas de forma explícita e separada, uma a uma, com a
referência bibliográfica completa no topo. É o formato mais completo e o
que melhor documenta o processo de leitura analítica de Severino.

## Mapa conceitual (formato CmapTools)

Entregável opcional, independente do tipo de fichamento escolhido: um
arquivo `.txt` com proposições no formato de importação de mapas conceituais
do CmapTools, cobrindo os principais termos/conceitos do texto.

**Formato:** cada linha é uma proposição com três campos separados por
tabulação (`\t`), sem cabeçalho:

```
CONCEITO 1<TAB>frase de ligação/verbo<TAB>CONCEITO 2
```

Exemplo (ilustrativo, não literal de nenhum texto específico):
```
LEITURA ANALÍTICA	organiza-se em	CINCO ETAPAS
ANÁLISE TEXTUAL	precede	ANÁLISE TEMÁTICA
PROBLEMATIZAÇÃO	depende de	POSICIONAMENTO DO LEITOR
```

**Como construir:**
- Extraia os conceitos principais do texto a partir do que já foi levantado
  nas etapas 1 e 2 (vocabulário-chave, tema, problema, tese, argumentos).
- Escreva os conceitos como substantivos ou expressões nominais curtas
  (não frases completas); por convenção do CmapTools, é comum usar
  caixa alta, mas isso é apenas estético — mantenha a formatação legível.
- A frase de ligação deve ser curta (um verbo ou expressão verbal) e
  expressar a relação real entre os dois conceitos, em suas próprias
  palavras — nunca copie frases inteiras do texto original.
- Cubra as relações mais importantes da unidade de leitura; para um
  capítulo ou artigo típico, algo entre 15 e 30 proposições costuma ser
  suficiente para capturar a estrutura conceitual sem sobrecarregar o mapa.
- Evite conceitos redundantes ou triplas que apenas repitam a mesma
  relação com sinônimos.
- Salve como arquivo `.txt` separado (não misture com o `.md` do
  fichamento), com um nome como `mapa-conceitual-[título].txt`.

## Template do arquivo .md

Adapte conforme o tipo de fichamento escolhido, mas sempre inclua a
referência no topo:

```markdown
# Fichamento — [Título do texto]

**Referência (ABNT):** SOBRENOME, Nome. *Título*. Edição. Cidade: Editora, Ano.
**Unidade de leitura:** [capítulo/seção/páginas fichadas]

## 1. Análise textual
- Autor:
- Vocabulário/conceitos-chave:
- Referências a esclarecer:

## 2. Análise temática
- Tema:
- Problema:
- Tese:
- Argumentos principais:
- Argumentos secundários:
- Conclusão:

## 3. Análise interpretativa (crítica externa)
- Pressupostos do autor:
- Hipóteses/doutrinas com que se identifica ou a que se contrapõe:
- Situação no debate/tradição de pensamento:
- Comparações com outros autores (se houver):

## 4. Problematização
- Questionamentos levantados:
- Novos problemas percebidos a partir da leitura:

## 5. Síntese pessoal (crítica interna + avaliação)
- O problema foi bem formulado?
- A tese é, de fato, solução do problema proposto?
- Os argumentos demonstram a solução?
- Os argumentos são válidos e as informações verificáveis?
- Originalidade e contribuição:
- Posição pessoal do leitor:

## Orientações para resenha/resumo crítico
*(apenas nos formatos e/f — resenha completa e analítico integral)*
- Pressupostos possíveis para avaliar:
- Estado da arte / debate externo ao texto:
- Autores ou correntes para comparação:
- Questionamentos sugeridos:
- Possíveis furos na coerência interna:
- Pontos de originalidade a considerar:
- Eixos sugeridos para posicionamento pessoal:
```

Para o formato (a), (b), (c) e (d), use apenas as seções correspondentes
do template (bibliográfico → só a referência e a estrutura da obra;
citações → lista de trechos com página; resumo indicativo → assunto,
problema e tese em texto conciso; resumo informativo → finalidade,
metodologia, resultados e conclusões), mas ainda assim baseie o conteúdo no
que foi levantado nas etapas 1 e 2. A seção "Orientações para
resenha/resumo crítico" não entra nesses formatos.

Para os formatos (e) e (f), preencha as seções 3, 4 e 5 e a seção de
Orientações conforme o modo de condução escolhido — o documento gerado
segue sempre a estrutura completa das cinco etapas, mudando apenas a
origem do conteúdo:
- **Modo 1 (diálogo):** as seções 3, 4 e 5 registram as respostas e
  posições que o usuário deu durante a entrevista; a seção de Orientações
  registra as sugestões que o Claude ofereceu ao longo da conversa, como
  referência de apoio.
- **Modo 2 (sugestões):** a seção de Orientações é o conteúdo principal
  gerado pelo Claude, com espaço logo abaixo de cada item para o usuário
  preencher; as seções 3, 4 e 5 ficam como campos em aberto para o usuário
  desenvolver depois, a partir dessas orientações.
- **Modo 3 (método direto):** as seções 3 e 4 são preenchidas diretamente
  pelo Claude como leitura especializada; na seção 5, a avaliação de
  coerência interna e a originalidade também são preenchidas pelo Claude,
  mas o campo "posição pessoal do leitor" fica em aberto para o usuário.

## Cuidados

- Nunca reproduza passagens longas do texto original (respeite limites de
  citação — poucas palavras por trecho, uma citação por fonte quando
  possível). Prefira parafrasear.
- Não invente dados biográficos do autor ou conteúdo que não esteja no
  texto fornecido; se não souber, deixe o campo em aberto, pesquise antes
  de preencher, ou registre sua dúvida ou lacuna no relatório final.
- Sempre confirme o nome do arquivo/título antes de gerar, se o usuário não
  tiver indicado um.
- Se o texto original não estiver em português, nunca produza uma tradução
  completa dele como parte do fichamento — isso reproduziria uma obra
  protegida por direitos autorais. O apoio ao usuário vem da densidade da
  paráfrase em português (ajustada ao nível de compreensão declarado), não
  de uma tradução à parte.
