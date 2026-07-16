# kit_leitura_academica

Coleção de skills para o Claude voltadas ao estudo e à análise de textos
acadêmicos, desenvolvidas para uso em contexto de ensino e pesquisa.

## Skills

| Skill | O que faz | Gatilho típico |
|---|---|---|
| [`leitura-analitica-severino/`](./leitura-analitica-severino/) | Conduz a leitura analítica de um texto acadêmico e gera um fichamento, seguindo o método de Antônio Joaquim Severino (SEVERINO, Antônio Joaquim. _Metodologia do trabalho científico_. 24. ed. rev. e ampl. São Paulo: Cortez, 2017.). Entrega um documento de análise para consulta posterior. | "Quero fazer uma leitura analítica desse texto" |
| [`tutor-de-texto/`](./tutor-de-texto/) | Conduz uma sessão de estudo interativa e conversacional, ponto a ponto, até que a pessoa consiga explicar o núcleo do artigo com as próprias palavras. Foco no processo de tutoria, não apenas no documento final. | "Quero usar o tutor de leitura com esse texto" |
| [`leitura-guiada/`](./leitura-guiada/) | Acompanha o leitor numa leitura sequencial do texto, seção por seção, na própria ordem em que ele se desenrola — centrada no leitor e no seu contexto, não num método de análise nem numa reorganização pedagógica do conteúdo. | "Quero fazer uma leitura guiada com esse texto" |

As três skills são complementares e podem ser usadas em combinação ou
isoladamente, conforme o objetivo:
- `leitura-guiada` é útil para acompanhar uma primeira leitura do texto na
  própria ordem em que ele se desenrola, adaptada ao contexto do leitor;
- `tutor-de-texto` reorganiza o conteúdo numa sequência pedagógica própria,
  para quem quer dominar o núcleo do artigo antes de mais nada;
- `leitura-analitica-severino` produz o registro formal de análise
  (fichamento), depois que o texto já foi trabalhado ou de forma
  independente, para quem já tem domínio de leitura acadêmica.

## Estrutura do repositório

```
kit_leitura_academica/
├── README.md                          # este arquivo
├── LICENSE                            # MIT
├── leitura-analitica-severino/
│   ├── SKILL.md
│   └── README.md
├── tutor-de-texto/
│   ├── SKILL.md
│   └── README.md
└── leitura-guiada/
    ├── SKILL.md
    └── README.md
```

Cada skill é independente e pode ser empacotada (`.skill`/`.zip`) e
instalada separadamente a partir da sua própria pasta.

## Instalação

Para usar uma skill no Claude, copie a pasta correspondente (contendo o
`SKILL.md`) para o diretório de skills do usuário, ou gere um pacote
`.skill`/`.zip` a partir dela para distribuição/instalação.

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
