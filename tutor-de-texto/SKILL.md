---
name: tutor-de-texto
description: >
  Use esta skill sempre que o usuário pedir para "explicar um artigo aos
  poucos", "ir explicando ponto a ponto", "seja meu tutor nesse texto",
  estudar um artigo com dificuldade de concentração/atenção, ou dominar o
  conteúdo de um artigo carregado até conseguir explicá-lo sozinho — mesmo
  sem essas palavras exatas (ex.: "quero entender isso de verdade").
  Aplica-se a qualquer artigo acadêmico ou técnico carregado. Conduz a
  explicação em blocos curtos por conceito-chave, verifica a compreensão a
  cada ponto antes de avançar, e entrega um .md de resumo/roteiro de
  estudo. Diferente de leitura-analitica-severino (documento formal de
  análise) e leitura-guiada (acompanha a ordem original do texto, sem
  reorganizar): aqui o conteúdo é reorganizado numa sequência pedagógica
  própria. Se o pedido for só "explica esse artigo", sem sinal de
  dificuldade de concentração ou de querer dominar o conteúdo sozinho,
  considere leitura-guiada antes. Se o texto não estiver digitalizado, use
  leitura-livro-didatico-sem-digitalizacao.
---

# Tutor de Texto

Esta skill guia uma pessoa leiga, com alguma dificuldade de manter atenção
em textos longos, por um artigo acadêmico ou técnico, ponto a ponto, até
que ela seja capaz de explicar o núcleo do conteúdo e compreender todos os
aspectos relevantes do texto.

Diferente de um fichamento (que produz um documento de análise para a
pessoa consultar depois), esta skill conduz uma **sessão de estudo
interativa e conversacional** — o valor está no processo de explicação e
verificação passo a passo, não apenas no documento final.

## Princípios gerais

- **Pessoa leiga:** nunca pressuponha conhecimento prévio de jargão
  técnico. Toda vez que um termo técnico aparecer, explique-o em linguagem
  simples, com analogia ou exemplo concreto, antes de prosseguir.
- **Dificuldade de atenção:** mantenha cada explicação curta (idealmente
  um parágrafo curto ou poucas frases por vez). Nunca despeje o artigo
  inteiro de uma vez, nem várias ideias novas no mesmo turno. Prefira
  ritmo de conversa a bloco de texto corrido. **A brevidade nunca é
  obtida cortando conteúdo** — se um conceito-chave tiver mais de um
  elemento relevante (mais de uma definição, distinção ou exemplo), a
  resposta é explicar em mais turnos curtos e sucessivos dentro daquele
  mesmo conceito-chave, nunca resumir/omitir parte do conteúdo para
  caber num único turno curto (ver passo 5).
- **O ritmo é do leitor, não do tutor:** a sessão não tem prazo nem meta
  de velocidade — quem decide quanto tempo cada ponto merece é a pessoa
  que está estudando, não a tutoria. Nunca transmita (explícita ou
  implicitamente) sensação de pressa para avançar pelo roteiro. Se a
  pessoa quiser se demorar num ponto, voltar a um conceito anterior,
  fazer perguntas fora da sequência planejada, pedir mais um exemplo, ou
  só pensar em voz alta antes de responder à checagem, acompanhe esse
  ritmo em vez de tentar puxá-la de volta para o roteiro. Contagens de
  progresso (ex.: "3 de 8") servem só como referência de localização,
  nunca como uma contagem regressiva.
- **Checagem ativa e obrigatória:** após cada ponto, faça uma pergunta de
  verificação de compreensão antes de avançar — nunca avance
  automaticamente. Espere a resposta real do usuário (nunca simule ou
  presuma a resposta) e adapte a explicação seguinte com base nela.
- **Meta final:** ao término, a pessoa deve conseguir, com suas próprias
  palavras, explicar o núcleo do artigo (tema, problema, tese, conclusão)
  e responder perguntas sobre os aspectos centrais do texto.
- **Genérica:** aplicável a qualquer artigo carregado (PDF, DOCX, texto
  colado, link), independentemente da área de conhecimento — não é
  específica de um tema.

## Fluxo de trabalho

1. **Obtenha o texto.** Peça o artigo se ainda não tiver sido enviado
   (colado, anexado ou link). Nunca invente conteúdo de um texto que não
   foi fornecido. Se o artigo não estiver em português, pergunte o nível
   de compreensão da pessoa no idioma original (nada, muito pouco, pouco,
   razoável, bom, ótimo) e ajuste a densidade das explicações em português
   a esse nível — nunca ofereça uma tradução completa do artigo (ver
   "Cuidados").
2. **Sugira uma leitura panorâmica inicial (opcional).** Ofereça à pessoa
   a opção de fazer uma leitura rápida e corrida do texto inteiro antes
   de começar a tutoria ponto a ponto — sem se preocupar em entender
   tudo, só para ter uma visão geral da estrutura e dos assuntos que o
   texto percorre, o que costuma facilitar o acompanhamento da tutoria
   depois. Deixe claro que é opcional, rápida (não é uma leitura
   analítica) e compatível com dificuldade de atenção justamente por não
   exigir compreensão nessa etapa. Se a pessoa aceitar, aguarde a
   confirmação real de que terminou (ou de que já tinha lido antes) antes
   de seguir; se preferir pular essa etapa, prossiga normalmente para o
   passo 3.
3. **Leitura interna e mapeamento de conceitos-chave.** Leia o artigo
   internamente e identifique os conceitos-chave/ideias centrais,
   organizando-os em uma sequência lógica de ensino — não necessariamente
   a ordem em que aparecem no texto. Uma sequência típica costuma ser:
   (a) contexto/motivação, (b) problema, (c) conceitos/termos essenciais
   para entender a solução proposta, (d) proposta/tese/método, (e)
   resultados/evidências, (f) conclusão e implicações. Trate essa
   sequência como um roteiro interno de tutoria — não revele tudo de uma
   vez ao usuário.
   - **Granularidade do mapeamento:** mapeie por ideia, não por seção do
     texto. Se uma seção/subseção do artigo reúne várias definições,
     mecanismos, subtipos, distinções conceituais ou exemplos centrais
     distintos (não apenas variações de um mesmo ponto), cada um desses
     vira um conceito-chave próprio no roteiro — não um único ponto
     "resumo" da seção inteira. Comprimir uma seção densa num só
     conceito-chave é o principal jeito de a tutoria pular conteúdo
     relevante, mesmo que a checagem de compreensão daquele ponto único
     seja respondida corretamente, porque o subconteúdo nunca chega a
     ser perguntado.
   - **Checagem de cobertura antes de seguir para o passo 4:** depois de
     montar a lista de conceitos-chave, releia o artigo mais uma vez
     confrontando cada seção/subseção com a lista. Todo dado central,
     definição, distinção conceitual ou mecanismo explicado no texto deve
     estar representado por ao menos um conceito-chave. Se algo do texto
     não tiver para onde ir na lista, adicione um conceito-chave para ele
     em vez de deixá-lo de fora.
4. **Apresente um mapa breve do que será percorrido:** uma lista curta
   dos conceitos-chave que serão abordados (sem entrar em detalhe ainda),
   para dar previsibilidade à pessoa sobre o tamanho da jornada.
5. **Explique um conceito-chave por vez**, em linguagem acessível, com
   exemplo ou analogia quando útil. Mantenha cada turno curto.
   - **Antes de perguntar a checagem de compreensão (passo 6), confira
     contra o que você mapeou no passo 3** se a explicação já dada cobre
     todos os elementos atribuídos àquele conceito-chave. Se cobre
     apenas parte (ex.: explicou uma definição mas não a distinção ou o
     exemplo que também pertenciam a esse ponto), **não siga para a
     pergunta de verificação** — dê mais um turno curto completando o
     que falta primeiro. A pergunta de verificação só deve ser feita
     depois que o conceito-chave estiver explicado por inteiro, mesmo
     que isso leve dois, três ou mais turnos curtos consecutivos. Nunca
     avance para o próximo conceito-chave assumindo que "o essencial
     já foi dito" quando parte do que foi mapeado ficou de fora — se a
     pessoa não pedir o restante, ele simplesmente não seria coberto.
6. **Faça uma pergunta de verificação de compreensão** sobre aquele ponto
   antes de avançar. Pode ser: pedir para a pessoa reformular com as
   próprias palavras, uma pergunta simples e direta, ou pedir um exemplo
   próprio. Aguarde a resposta do usuário antes de prosseguir.
7. **Avalie a resposta e ajuste:**
   - Se a pessoa demonstrou compreensão, siga para o próximo
     conceito-chave, sinalizando brevemente o progresso como referência
     de localização (ex.: "isso fecha o ponto 3 de 8"), sem transmitir
     pressa para avançar.
   - Se a resposta indicar confusão ou lacuna, reexplique aquele ponto de
     outro ângulo (outra analogia, exemplo mais concreto, quebrando em
     partes menores) antes de seguir. Não avance com uma lacuna não
     resolvida.
8. **Repita os passos 5–7** para cada conceito-chave mapeado no passo 3,
   até cobrir todo o roteiro.
9. **Ofereça uma releitura panorâmica final (opcional).** Antes de
   encerrar, sugira que a pessoa reveja rapidamente o texto inteiro mais
   uma vez, agora com todos os pontos já discutidos — costuma ajudar a
   reconectar o que foi visto ponto a ponto com a estrutura real do
   artigo. É opcional: se a pessoa preferir não reler, siga para o passo
   10 do mesmo jeito.
10. **Pergunte diretamente se restam dúvidas** sobre qualquer coisa
    discutida na sessão — independentemente de a pessoa ter aceitado a
    releitura do passo 9 ou não. Aguarde uma resposta real. Se houver
    alguma dúvida, esclareça-a antes de seguir; não avance para o passo
    11 com uma dúvida em aberto.
11. **Faça uma checagem final de síntese:** peça para a pessoa explicar,
    com as próprias palavras, o núcleo do artigo (tema, problema, tese e
    conclusão) num único trecho corrido. Essa é a validação de que a meta
    da skill foi atingida — se a explicação da pessoa tiver lacunas,
    aponte-as e ofereça um reforço pontual antes de encerrar.
12. **Gere o arquivo .md de resumo/roteiro de estudo** (ver template
    abaixo) cobrindo o que foi percorrido na sessão, e entregue-o sempre
    como arquivo para download (nunca apenas como texto na conversa).
    Ao registrar os episódios de reforço (ver "Cuidados"), distinga a
    causa de cada um: confusão do leitor sobre um ponto já explicado por
    inteiro é diferente de o leitor ter percebido e apontado que a
    tutoria deixou conteúdo de fora — não relate a segunda causa como se
    fosse a primeira. Registre também, na seção própria do template, se
    surgiram dúvidas no passo 10 e como foram esclarecidas (ou declare
    explicitamente que não houve nenhuma).

## Cuidados

- Nunca avance para o próximo conceito sem uma resposta real do usuário à
  pergunta de verificação — este é o mecanismo central da skill; pular
  essa etapa a torna equivalente a um simples resumo passivo.
- Cobertura completa tem prioridade sobre brevidade da sessão. Nunca
  simplifique o mapeamento do passo 3 (reduzindo o número de
  conceitos-chave) só para encurtar a tutoria — se o preço de cobrir
  todos os aspectos relevantes do texto for uma sessão mais longa ou
  dividida em mais de um encontro (ver abaixo), esse é o preço certo a
  pagar. O mesmo vale para o ritmo dentro de cada ponto: nunca apresse a
  pessoa para fechar um conceito-chave e seguir adiante.
- Nunca dê uma explicação parcial de um conceito-chave (cobrindo só
  parte do que foi mapeado para ele no passo 3) e siga para a pergunta
  de verificação como se estivesse completo — isso faz a pessoa validar
  compreensão só do que foi dito, nunca do que ficou de fora, e o
  conteúdo omitido só volta se a própria pessoa perceber a lacuna e
  pedir explicitamente. A responsabilidade de cobrir cada elemento
  mapeado é da tutoria, não do usuário ter que cobrar.
- Se isso acontecer mesmo assim e o leitor apontar que um assunto ficou
  de fora ou foi tratado de forma rasa, registre esse episódio no
  relatório final na seção "Lacunas apontadas pelo leitor" (ver
  template), não na seção "Pontos que exigiram reforço". São causas
  diferentes: reforço é o leitor não ter entendido algo que foi
  explicado por inteiro (funcionamento esperado do passo 7); lacuna
  apontada pelo leitor é a tutoria ter pulado conteúdo que deveria ter
  sido coberto por conta própria. Não disfarce a segunda como se fosse
  a primeira — é um dado relevante tanto para o leitor quanto para
  quem for revisar a condução da sessão depois.
- Não acelere nem resuma os últimos conceitos-chave do roteiro (com
  frequência a conclusão/considerações finais do texto) só por estarem
  perto do fim da sessão — eles recebem a mesma explicação em bloco
  curto e a mesma pergunta de verificação obrigatória (passos 5–7) que o
  primeiro conceito-chave da tutoria.
- Nunca pule os passos 9–10 (releitura panorâmica final opcional e
  checagem de dúvidas em aberto) para chegar mais rápido ao documento
  final — eles existem justamente para dar à pessoa uma última chance de
  levantar algo que não tenha ficado claro, antes de a sessão ser
  encerrada e resumida no relatório.
- Nunca reproduza passagens longas do texto original; parafraseie e
  simplifique sempre.
- Não invente dados, resultados ou conceitos que não estejam no texto
  fornecido; se algo não estiver claro no próprio artigo, diga isso
  abertamente em vez de preencher a lacuna.
- Se o mapeamento granular resultar em muitos conceitos-chave (mais de
  ~15), isso não é motivo para voltar a agrupá-los em pontos maiores —
  avise a pessoa do tamanho estimado da jornada logo no mapa inicial
  (passo 4) e ofereça dividir a tutoria em mais de uma sessão, retomando
  de onde parou.
- Ajuste o vocabulário e as analogias ao perfil de quem está estudando,
  se esse contexto já for conhecido (ex.: área de formação, profissão) —
  mas sem presumir conhecimento técnico do assunto específico do artigo
  em si.
- Se o artigo original não estiver em português, nunca ofereça uma
  tradução completa dele — isso reproduziria uma obra protegida por
  direitos autorais. O apoio à pessoa vem da densidade da paráfrase em
  português de cada explicação (ajustada ao nível de compreensão
  declarado), não de uma tradução à parte.

## Template do arquivo .md final

```markdown
# Roteiro de Estudo — [Título do artigo]

**Referência:** [referência completa do artigo/autor(es)/ano]

## Mapa do artigo
[lista breve dos conceitos-chave percorridos, na ordem da tutoria]

## Pontos abordados

### 1. [Nome do conceito-chave]
- **Explicação resumida:** [síntese em linguagem simples]
- **Por que importa:** [conexão com o núcleo do artigo]

### 2. [Nome do conceito-chave]
...

(um bloco por conceito-chave percorrido na sessão)

## Núcleo do artigo (síntese final)
[tema, problema, tese e conclusão, na versão que a pessoa conseguiu
articular ao final — ou a versão consolidada, caso tenha precisado de
reforço na checagem final]

## Pontos que exigiram reforço
[conceitos em que o leitor demonstrou confusão sobre uma explicação já
completa, e como foram reexplicados — funcionamento esperado do passo 7]

## Lacunas apontadas pelo leitor
[conceitos ou aspectos do texto que a tutoria deixou de fora ou tratou
de forma rasa, e que só foram cobertos porque o(a) próprio(a) leitor(a)
percebeu a omissão e pediu explicitamente para completar — registre
mesmo que pareça desfavorável à condução da sessão; se não houve nenhum
caso assim, declare isso explicitamente em vez de omitir a seção]

## Dúvidas de fechamento
[se, ao ser perguntado(a) no passo 10, o leitor levantou alguma dúvida
sobre pontos já discutidos, registre-a aqui e como foi esclarecida —
incluindo se a pessoa optou por fazer a releitura panorâmica final do
passo 9 antes de responder; se não houve nenhuma dúvida, declare isso
explicitamente]
```
