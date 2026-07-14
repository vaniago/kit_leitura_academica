---
name: tutor-de-texto
description: "Use esta skill sempre que o usuário pedir para \"explicar um artigo aos poucos\", \"ir explicando ponto a ponto\", \"seja meu tutor nesse texto\",  estudar um artigo com dificuldade de concentração/atenção, ou pedir para dominar o conteúdo de um artigo carregado (PDF, DOCX, texto colado) até conseguir explicá-lo sozinho — mesmo que o usuário não use essas palavras exatas (ex.: \"me ajuda a estudar isso aos poucos\", \"explica esse artigo como se eu não soubesse nada do assunto\", \"quero entender isso de verdade antes de acabar\"). Aplica-se a qualquer artigo acadêmico ou técnico carregado pelo usuário, independentemente do tema ou área de conhecimento. Sempre conduz a explicação em blocos curtos organizados por conceito-chave, verifica ativamente a compreensão do usuário a cada ponto antes de avançar, e entrega ao final um arquivo .md de resumo/roteiro de estudo."
---

# Tutor de Texto

Esta skill guia uma pessoa leiga, com alguma dificuldade de manter atenção
em textos longos, por um artigo acadêmico ou técnico, ponto a ponto, até
que ela seja capaz de explicar o núcleo do conteúdo e compreender todos os
aspectos relevantes do texto.

Diferente de um fichamento (que produz um documento de análise para o
leitor consultar depois), esta skill conduz uma **sessão de estudo
interativa e conversacional** — o valor está no processo de explicação e
verificação passo a passo, não apenas no documento final.

## Princípios gerais

- **Pessoa leiga:** nunca pressuponha conhecimento prévio de jargão
  técnico. Toda vez que um termo técnico aparecer, explique-o em linguagem
  simples, com analogia ou exemplo concreto, antes de prosseguir.
- **Dificuldade de atenção:** mantenha cada explicação curta (idealmente
  um parágrafo curto ou poucas frases por vez). Nunca despeje o artigo
  inteiro de uma vez, nem várias ideias novas no mesmo turno. Prefira
  ritmo de conversa a bloco de texto corrido.
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
   foi fornecido.
2. **Leitura interna e mapeamento de conceitos-chave.** Leia o artigo
   internamente e identifique os conceitos-chave/ideias centrais,
   organizando-os em uma sequência lógica de ensino — não necessariamente
   a ordem em que aparecem no texto. Uma sequência típica costuma ser:
   (a) contexto/motivação, (b) problema, (c) conceitos/termos essenciais
   para entender a solução proposta, (d) proposta/tese/método, (e)
   resultados/evidências, (f) conclusão e implicações. Trate essa
   sequência como um roteiro interno de tutoria — não revele tudo de uma
   vez ao usuário.
3. **Apresente um mapa breve do que será percorrido:** uma lista curta
   dos conceitos-chave que serão abordados (sem entrar em detalhe ainda),
   para dar previsibilidade à pessoa sobre o tamanho da jornada.
4. **Explique um conceito-chave por vez**, em linguagem acessível, com
   exemplo ou analogia quando útil. Mantenha o bloco curto.
5. **Faça uma pergunta de verificação de compreensão** sobre aquele ponto
   antes de avançar. Pode ser: pedir para a pessoa reformular com as
   próprias palavras, uma pergunta simples e direta, ou pedir um exemplo
   próprio. Aguarde a resposta do usuário antes de prosseguir.
6. **Avalie a resposta e ajuste:**
   - Se a pessoa demonstrou compreensão, siga para o próximo
     conceito-chave, sinalizando brevemente o progresso (ex.: "boa,
     vamos para o próximo ponto — 3 de 8").
   - Se a resposta indicar confusão ou lacuna, reexplique aquele ponto de
     outro ângulo (outra analogia, exemplo mais concreto, quebrando em
     partes menores) antes de seguir. Não avance com uma lacuna não
     resolvida.
7. **Repita os passos 4–6** para cada conceito-chave mapeado no passo 2,
   até cobrir todo o roteiro.
8. **Faça uma checagem final de síntese:** peça para a pessoa explicar,
   com as próprias palavras, o núcleo do artigo (tema, problema, tese e
   conclusão) num único trecho corrido. Essa é a validação de que a meta
   da skill foi atingida — se a explicação da pessoa tiver lacunas,
   aponte-as e ofereça um reforço pontual antes de encerrar.
9. **Gere o arquivo .md de resumo/roteiro de estudo** (ver template
   abaixo) cobrindo o que foi percorrido na sessão, e entregue-o sempre
   como arquivo para download (nunca apenas como texto na conversa).

## Cuidados

- Nunca avance para o próximo conceito sem uma resposta real do usuário à
  pergunta de verificação — este é o mecanismo central da skill; pular
  essa etapa a torna equivalente a um simples resumo passivo.
- Nunca reproduza passagens longas do texto original; parafraseie e
  simplifique sempre.
- Não invente dados, resultados ou conceitos que não estejam no texto
  fornecido; se algo não estiver claro no próprio artigo, diga isso
  abertamente em vez de preencher a lacuna.
- Se o artigo for muito longo (mais de ~15 conceitos-chave), avise a
  pessoa do tamanho estimado da jornada logo no mapa inicial (passo 3), e
  ofereça dividir a tutoria em mais de uma sessão, retomando de onde
  parou.
- Ajuste o vocabulário e as analogias ao perfil de quem está estudando,
  se esse contexto já for conhecido (ex.: área de formação, profissão) —
  mas sem presumir conhecimento técnico do assunto específico do artigo
  em si.

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
[conceitos em que houve confusão inicial e como foram reexplicados — útil
para revisão futura]
```