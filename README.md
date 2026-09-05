# kit_leitura_academica

**Kit de skills de IA para leitura acadêmica, científica e literária no
Claude** (Claude Code e claude.ai) — sete habilidades que ensinam e
acompanham métodos de estudo de texto (fichamento, letramento literário,
leitura crítica de artigos) em vez de substituir a leitura por um resumo
pronto. Desenvolvido para uso em contexto de ensino e pesquisa, em
português.

## Motivação

O estudo de textos acadêmicos exige metodologia.
Com o avanço dos LLM (large language models de inteligência artificial), 
tornou-se comum o **_lsl_** - ler sem ler - em que a pessoa lança o texto 
para o LLM e colhe um resumo, um fichamento, sem se envolver com o processo 
de pensamento que leva ao produto acadêmico. 

Esse kit contém habilidades (skills) de leitura de diversos tipos, baseadas
em métodos de estudo reconhecidos — como o fichamento de Antônio Joaquim
Severino, o método das três passadas de S. Keshav (*How to Read a Paper*)
e o letramento literário de Rildo Cosson — adaptados para uso conversacional
com IA. Elas buscam cobrir diferentes necessidades de quem lê, de modo a
permitir um processo interativo e dialogal do entendimento, interpretação e
produção a partir da leitura, para que a pessoa possa efetivamente aprender
ao ler.

Embora essas habilidades (skills) se dirijam ao público em geral, 
elas foram pensadas para estudantes de ensino médio e início de ensino superior e, 
por isso, partem de uma visão didática, que pode ser dispensada por pessoas 
com mais experiência em leitura.

## Skills

| Skill | O que faz | Gatilho típico |
|---|---|---|
| [`triagem-de-leitura/`](./triagem-de-leitura/) | Não conduz leitura — ajuda a escolher, entre as demais skills do kit, qual encaixa melhor com o texto e o objetivo de quem lê. Útil para quem não sabe por qual das seis começar. | "Não sei qual skill de leitura usar pra esse texto" |
| [`tutor-de-texto/`](./tutor-de-texto/) | Conduz uma sessão de estudo interativa e conversacional, ponto a ponto, até que a pessoa consiga explicar o núcleo do artigo com as próprias palavras. Foco no processo de tutoria, não apenas no documento final. | "Quero usar o tutor de leitura com esse texto" |
| [`leitura-guiada/`](./leitura-guiada/) | Acompanha o leitor numa leitura sequencial do texto, seção por seção, na própria ordem em que ele se desenrola — centrada no leitor e no seu contexto, não num método de análise nem numa reorganização pedagógica do conteúdo. | "Quero fazer uma leitura guiada com esse texto" |
| [`leitura-analitica-severino/`](./leitura-analitica-severino/) | Conduz a leitura analítica de um texto acadêmico e gera um fichamento, seguindo o método de Antônio Joaquim Severino (SEVERINO, Antônio Joaquim. _Metodologia do trabalho científico_. 24. ed. rev. e ampl. São Paulo: Cortez, 2017.). Entrega um documento de análise para consulta posterior. | "Quero fazer uma leitura analítica desse texto" |
| [`leitura-cientifica-keshav/`](./leitura-cientifica-keshav/) | Acompanha a leitura de um único artigo científico usando o método das três passadas de S. Keshav (*How to Read a Paper*, 2007) — panorama, compreensão do conteúdo e leitura crítica, com a última calibrada pelo nível de experiência de quem lê. | "Quero aplicar o método das três passadas nesse paper" |
| [`leitura-literaria-cosson/`](./leitura-literaria-cosson/) | Acompanha o estudo de uma obra literária (poema, conto, romance, crônica, peça) usando o letramento literário de Rildo Cosson (COSSON, Rildo. _Letramento literário: teoria e prática_. São Paulo: Contexto, 2009) — sequência básica (motivação, introdução, leitura, interpretação) ou expandida (com contextualização e expansão), sempre deixando a interpretação a cargo da própria pessoa. | "Quero estudar esse poema com o método do Cosson" |
| [`leitura-livro-didatico-sem-digitalizacao/`](./leitura-livro-didatico-sem-digitalizacao/) | Acompanha o leitor na leitura de um capítulo de livro didático impresso quando não há versão digitalizada do texto — o Claude não tem acesso ao conteúdo além do que o leitor relatar, e gera um relatório de sessão com evidências de leitura real, pronto para anexar como tarefa. | "Vou fazer minha leitura semanal, só tenho o livro físico" |

As sete skills são complementares e podem ser usadas em combinação ou
isoladamente, conforme o objetivo:
- `triagem-de-leitura` não é uma skill de leitura em si — é o ponto de
  entrada para quem tem um texto mas não sabe qual das outras seis
  encaixa melhor; faz algumas perguntas e recomenda uma delas;
- `tutor-de-texto` reorganiza o conteúdo numa sequência pedagógica própria,
  para quem quer dominar o núcleo do artigo antes de mais nada;
- `leitura-guiada` é útil para acompanhar uma primeira leitura do texto na
  própria ordem em que ele se desenrola, adaptada ao contexto do leitor;
- `leitura-analitica-severino` produz o registro formal de análise
  (fichamento), depois que o texto já foi trabalhado ou de forma
  independente, para quem já tem domínio de leitura acadêmica;
- `leitura-cientifica-keshav` é específica para um único artigo/paper
  científico, estruturada em três releituras sucessivas de profundidade
  crescente (panorama, compreensão, leitura crítica), não em revisão de
  literatura comparando várias fontes;
- `leitura-literaria-cosson` é específica para texto literário, não busca
  extrair um argumento ou tese (isso é papel das demais skills, pensadas
  para texto acadêmico/técnico/científico), e sim formar a capacidade da
  pessoa de interpretar a obra por conta própria;
- `leitura-livro-didatico-sem-digitalizacao` é a alternativa às demais
  quando o texto não está digitalizado — todas as outras partem de um
  texto colado, anexado ou por link.
  
## Estrutura do repositório

```
kit_leitura_academica/
├── README.md                          # este arquivo
├── LICENSE                            # MIT
├── triagem-de-leitura/
│   ├── SKILL.md
│   └── README.md
├── tutor-de-texto/
│   ├── SKILL.md
│   └── README.md
├── leitura-guiada/
│   ├── SKILL.md
│   └── README.md
├── leitura-analitica-severino/
│   ├── SKILL.md
│   └── README.md
├── leitura-cientifica-keshav/
│   ├── SKILL.md
│   └── README.md
├── leitura-literaria-cosson/
│   ├── SKILL.md
│   └── README.md
└── leitura-livro-didatico-sem-digitalizacao/
    ├── SKILL.md
    └── README.md
```

Cada skill funciona por conta própria — nenhuma delas depende de outra
estar instalada para operar — e pode ser empacotada (`.skill`/`.zip`) e
instalada separadamente a partir da sua própria pasta.

## Instalação

### Antes de tudo: baixando os arquivos pelo navegador (sem usar Git)

Quem não é acostumado com GitHub não precisa aprender a mexer com ele —
dá para conseguir os arquivos direto pelo navegador, sem instalar nada
além de um programa de descompactar (Windows e macOS já vêm com um).

**Para baixar o kit inteiro (as sete skills de uma vez):**

1. Nesta página do repositório no GitHub, clique no botão verde **Code**
   (perto do topo da página).
2. Clique em **Download ZIP**.
3. Extraia o arquivo baixado:
   - **Windows:** clique com o botão direito no `.zip` → **Extrair
     tudo**.
   - **macOS:** dê duplo clique no `.zip`.
4. Você terá uma pasta (algo como `kit_leitura_academica-main`) com uma
   subpasta para cada skill (`triagem-de-leitura/`, `tutor-de-texto/`
   etc.) — cada uma dessas subpastas é a "pasta da skill" mencionada nas
   instruções mais abaixo.

**Para baixar só uma skill específica** (por exemplo, só
`leitura-guiada/`), sem precisar do kit inteiro:

- **Mais simples:** baixe o kit inteiro como acima e use apenas a
  subpasta da skill desejada; as demais podem ser ignoradas ou
  apagadas.
- **Sem baixar o kit inteiro:** abra a pasta da skill neste repositório
  no GitHub (por exemplo,
  `https://github.com/vaniago/kit_leitura_academica/tree/main/leitura-guiada`),
  copie esse endereço, cole em
  [download-directory.github.io](https://download-directory.github.io)
  e clique para baixar. Isso gera um `.zip` já contendo só aquela pasta
  — pode pular direto para o passo de upload na Opção 1 abaixo, sem
  precisar compactar nada de novo.

  > `download-directory.github.io` é uma ferramenta gratuita e de
  > código aberto mantida pela comunidade (não é da Anthropic nem do
  > GitHub) que baixa apenas uma subpasta de um repositório público.

**Recomendado: baixe o kit completo.** As seis skills de leitura cobrem
situações diferentes (texto acadêmico genérico, artigo científico, obra
literária, livro didático sem digitalização, foco no processo de tutoria,
foco no fichamento formal), e não dá para saber de antemão qual vai
encaixar melhor com um texto ou um jeito de estudar — é por isso que o
kit inclui também a `triagem-de-leitura`, que ajuda a escolher entre elas
quando não estiver claro. Tendo o kit inteiro instalado, se uma skill não
estiver progredindo bem numa sessão, dá para simplesmente trocar para
outra sem precisar interromper o fluxo para ir buscar e instalar mais uma
pasta.

Ainda assim, cada skill é independente e pode ser instalada avulsa — por
exemplo, para quem só vai usar `leitura-cientifica-keshav` e prefere não
carregar as demais. Para usar uma skill no Claude, copie a pasta
correspondente (contendo o `SKILL.md`) para o diretório de skills do
usuário, ou gere um pacote `.skill`/`.zip` a partir dela para
distribuição/instalação.

**Opção 1 — pelo Claude no navegador (claude.ai):**

1. Se você usou `download-directory.github.io` acima, já tem o `.zip`
   pronto — pule para o passo 2. Senão, compacte a pasta da skill
   (contendo o `SKILL.md`) em um `.zip`:
   - **Windows:** clique com o botão direito na pasta → **Enviar para →
     Pasta compactada** (ou, no PowerShell: `Compress-Archive -Path
     .\leitura-guiada\* -DestinationPath .\leitura-guiada.zip`).
   - **macOS:** clique com o botão direito na pasta → **Comprimir**.
   - **Linux / terminal (macOS incluso):**
     ```
     cd leitura-guiada && zip -r ../leitura-guiada.zip .
     ```
2. No claude.ai, vá em **Configurações → Habilidades (Capabilities) →
   Adicionar habilidade**.
3. Faça o upload do `.zip` gerado.

**Opção 2 — copiar a pasta direto (Claude Code):**

1. Localize o diretório de skills do usuário: `~/.claude/skills/`
   (Linux/macOS) ou `%USERPROFILE%\.claude\skills\` no Windows — em
   ambos os casos, crie a pasta `skills` se ela ainda não existir.
2. Copie a pasta da skill desejada para dentro dele:
   - **Linux/macOS:**
     ```
     cp -r leitura-guiada ~/.claude/skills/
     ```
   - **Windows (PowerShell):**
     ```
     New-Item -ItemType Directory -Force -Path "$env:USERPROFILE\.claude\skills" | Out-Null
     Copy-Item -Recurse -Path .\leitura-guiada -Destination "$env:USERPROFILE\.claude\skills\"
     ```
3. Reinicie o Claude Code (ou abra uma nova sessão) para que a skill seja
   carregada.

**Opção 3 — empacotar como `.skill`/`.zip` para distribuir a terceiros:**

1. Compacte a pasta da skill do mesmo jeito da Opção 1 (no sistema
   operacional de quem estiver empacotando).
2. Compartilhe o arquivo gerado com quem for instalar.
3. Quem receber pode usar tanto a Opção 1 (upload pelo navegador) quanto
   a Opção 2 (pasta de skills local), conforme onde for usar o Claude e
   qual for o sistema operacional — o `.zip` funciona nos dois casos,
   em qualquer sistema.

## Licença

MIT — ver [LICENSE](./LICENSE).
