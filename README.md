# kit_leitura_academica

Coleção de skills para o Claude voltadas ao estudo e à análise de textos
acadêmicos, desenvolvidas para uso em contexto de ensino e pesquisa.

## Motivação

O estudo de textos acadêmicos exige metodologia. 
Com o avanço dos LLM (large language models de inteligência artificial), 
tornou-se comum o **_lsl_** - ler sem ler - em que a pessoa lança o texto 
para o LLM e colhe um resumo, um fichamento, sem se envolver com o processo 
de pensamento que leva ao produto acadêmico. 

Esse kit contém habilidades (skills) de leitura de diversos tipos, que buscam 
cobrir diferentes necessidades de quem lê, de modo a permitir um processo 
interativo e dialogal do entendimento, interpretação e produção a partir da 
leitura, para que a pessoa possa efetivamente aprender ao ler.

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
| [`leitura-literaria-cosson/`](./leitura-literaria-cosson/) | Acompanha o estudo de uma obra literária (poema, conto, romance, crônica, peça) usando o letramento literário de Rildo Cosson — sequência básica (motivação, introdução, leitura, interpretação) ou expandida (com contextualização e expansão), sempre deixando a interpretação a cargo da própria pessoa. | "Quero estudar esse poema com o método do Cosson" |
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

1. Compacte a pasta da skill (contendo o `SKILL.md`) em um `.zip`:
   ```
   cd leitura-guiada && zip -r ../leitura-guiada.zip .
   ```
2. No claude.ai, vá em **Configurações → Habilidades (Capabilities) →
   Adicionar habilidade**.
3. Faça o upload do `.zip` gerado.

**Opção 2 — copiar a pasta direto (Claude Code):**

1. Localize o diretório de skills do usuário: `~/.claude/skills/` (crie-o
   se ainda não existir).
2. Copie a pasta da skill desejada para dentro dele, por exemplo:
   ```
   cp -r leitura-guiada ~/.claude/skills/
   ```
3. Reinicie o Claude Code (ou abra uma nova sessão) para que a skill seja
   carregada.

**Opção 3 — empacotar como `.skill`/`.zip` para distribuir a terceiros:**

1. Compacte a pasta da skill do mesmo jeito da Opção 1.
2. Compartilhe o arquivo gerado com quem for instalar.
3. Quem receber pode usar tanto a Opção 1 (upload pelo navegador) quanto
   a Opção 2 (`~/.claude/skills/`), conforme onde for usar o Claude.

## Licença

MIT — ver [LICENSE](./LICENSE).
