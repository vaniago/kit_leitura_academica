# leitura-guiada

Skill para o Claude que acompanha o leitor numa leitura sequencial de um
texto acadêmico ou técnico, seção por seção, na própria ordem em que o
texto se desenrola.

## O que faz

Diferente do `leitura-analitica-severino` (que reorganiza a leitura em
cinco etapas metodológicas) e do `tutor-de-texto` (que reorganiza o
conteúdo numa sequência pedagógica própria), esta skill segue exatamente
o caminho que o texto percorre, centrada no leitor e no seu contexto:

1. Faz uma síntese inicial breve do texto, para aliviar a ansiedade de
   começar sem saber do que se trata.
2. Conduz uma entrevista breve sobre o motivo da leitura e o nível de
   expertise no tema.
3. Levanta o que o leitor já sabe sobre o assunto, antes de ler.
4. Acompanha a leitura seção por seção, explicando pré-requisitos sob
   demanda e checando a compreensão ao longo do caminho.
5. Ao final, compara o que o leitor sabia antes com o que consegue
   articular depois, e mostra o progresso de forma concreta.
6. Gera um arquivo `.md` com o relatório da sessão e recomendações de
   leitura complementar (de fundamentos e por interesse espontâneo).

Pensada especialmente para estudantes de ensino técnico ou médio, estudantes de
início de graduação, ou qualquer pessoa leiga no assunto do texto mas que
já lê e compreende texto normalmente.

## Instalação

**Opção 1 — pelo Claude no navegador (claude.ai):**

1. Compacte a pasta `leitura-guiada/` (contendo o `SKILL.md`) em um `.zip`:
   ```
   cd leitura-guiada && zip -r ../leitura-guiada.zip .
   ```
2. No claude.ai, vá em **Configurações → Habilidades (Capabilities) →
   Adicionar habilidade**.
3. Faça o upload do `.zip` gerado.

**Opção 2 — copiar a pasta direto (Claude Code):**

1. Localize o diretório de skills do usuário: `~/.claude/skills/` (crie-o
   se ainda não existir).
2. Copie a pasta para dentro dele:
   ```
   cp -r leitura-guiada ~/.claude/skills/
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
