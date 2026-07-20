# leitura-literaria-cosson

Skill para o Claude que acompanha o estudo de uma obra literária (poema,
conto, romance, crônica, peça) usando o letramento literário de Rildo
Cosson (*Letramento Literário: Teoria e Prática*, 2009).

## O que faz

Diferente do `leitura-cientifica-keshav` (artigo científico) e do
`leitura-guiada`/`leitura-analitica-severino` (texto acadêmico/técnico
argumentativo genérico), esta skill é específica para texto literário, e
não busca extrair um argumento ou tese, e sim formar a capacidade da
pessoa de interpretar a obra por conta própria.

1. Pergunta se a pessoa já conhece o método de Cosson; se não conhecer,
   explica as duas sequências possíveis antes de deixar escolher.
2. **Sequência básica (padrão):** motivação (conversa inicial sobre o
   tema da obra) → introdução (dados sobre autor e obra) → leitura →
   interpretação (impressão pessoal da pessoa sobre o que leu).
3. **Sequência expandida (opcional):** os mesmos três primeiros passos,
   com a interpretação desdobrada em primeira interpretação →
   contextualização (histórica, estilística, temática etc.) → segunda
   interpretação (aprofundamento num aspecto específico da obra) →
   expansão (relação com outras obras/experiências).
4. A etapa de Motivação pode ser pulada se já tiver sido feita
   presencialmente por um professor antes da sessão.
5. Gera um relatório `.md` da sessão com o que a pessoa produziu em cada
   etapa — nunca uma interpretação escrita pelo Claude.

O princípio central é que **a interpretação é da pessoa, não do Claude**:
o pedido mais comum e mais tentador aqui é "explica esse poema pra mim" —
a skill nunca cede a isso. Informação factual (dados biográficos,
contexto histórico, movimento literário) só entra na Introdução e na
Contextualização, sempre verificada, nunca inventada.

Pensada especialmente para estudantes de ensino médio e início de
graduação trabalhando leitura literária, mas serve para qualquer pessoa
estudando uma obra literária de forma acompanhada.

## Instalação

**Opção 1 — pelo Claude no navegador (claude.ai):**

1. Compacte a pasta `leitura-literaria-cosson/` (contendo o `SKILL.md`)
   em um `.zip`:
   ```
   cd leitura-literaria-cosson && zip -r ../leitura-literaria-cosson.zip .
   ```
2. No claude.ai, vá em **Configurações → Habilidades (Capabilities) →
   Adicionar habilidade**.
3. Faça o upload do `.zip` gerado.

**Opção 2 — copiar a pasta direto (Claude Code):**

1. Localize o diretório de skills do usuário: `~/.claude/skills/` (crie-o
   se ainda não existir).
2. Copie a pasta para dentro dele:
   ```
   cp -r leitura-literaria-cosson ~/.claude/skills/
   ```
3. Reinicie o Claude Code (ou abra uma nova sessão) para que a skill seja
   carregada.

**Opção 3 — empacotar como `.skill`/`.zip` para distribuir a terceiros:**

1. Compacte a pasta do mesmo jeito da Opção 1.
2. Compartilhe o arquivo gerado com quem for instalar.
3. Quem receber pode usar tanto a Opção 1 (upload pelo navegador) quanto
   a Opção 2 (`~/.claude/skills/`), conforme onde for usar o Claude.

## Licença

MIT — ver [LICENSE](../LICENSE) na raiz do repositório.
