# leitura-livro-didatico-sem-digitalizacao

Skill para o Claude que acompanha o leitor na leitura de um capítulo de
livro didático impresso, quando não há versão digitalizada do texto — o
livro está fisicamente com o leitor, e o Claude não tem acesso ao
conteúdo além do que o próprio leitor relatar durante a sessão.

## O que faz

Diferente das demais skills de leitura deste kit (pensadas para um texto
já digitalizado — colado, anexado ou por link), esta skill é
especificamente para quando só existe o livro físico. Ela transforma a
ausência de acesso ao texto numa vantagem pedagógica: em vez de tentar
verificar a leitura por fora, ancora a conversa na página física do
livro, tornando mais fácil realmente ler do que fabricar o relatório —
sem nunca perder de vista que a pedagogia vem antes da verificação.

1. Abre a sessão levantando livro, disciplina e capítulo, e delimita com
   o leitor qual parte será percorrida.
2. Acompanha a leitura relatada seção por seção: pede descrição da
   página, intercala perguntas ancoradas na localização física do livro,
   e pede sínteses periódicas para consolidar o que foi lido.
3. Explica termos e dúvidas conceituais com bom senso de professor — dá
   uma resposta mínima e honesta mesmo estando sem acesso ao texto, em
   vez de insistir secamente em "volta pro texto" sem dar nada em troca.
4. No fechamento, retoma as dúvidas que só receberam resposta mínima
   durante a leitura e as esclarece por completo, já que a leitura
   terminou e o texto pode não ter respondido ao interesse do leitor.
5. Gera um relatório `.md`, pronto para anexar como tarefa no ambiente
   virtual de aprendizagem (ex.: Moodle), com transcrição fiel das
   respostas do leitor — nunca um resumo reescrito pelo Claude.

Pensada especialmente para quem faz leitura escolar periódica de
capítulos de livro didático impresso, em qualquer disciplina (Filosofia,
Biologia, História etc.), sem ter o texto digitalizado à mão.

## Instalação

**Opção 1 — pelo Claude no navegador (claude.ai):**

1. Compacte a pasta `leitura-livro-didatico-sem-digitalizacao/` (contendo
   o `SKILL.md`) em um `.zip`:
   ```
   cd leitura-livro-didatico-sem-digitalizacao && zip -r ../leitura-livro-didatico-sem-digitalizacao.zip .
   ```
2. No claude.ai, vá em **Configurações → Habilidades (Capabilities) →
   Adicionar habilidade**.
3. Faça o upload do `.zip` gerado.

**Opção 2 — copiar a pasta direto (Claude Code):**

1. Localize o diretório de skills do usuário: `~/.claude/skills/` (crie-o
   se ainda não existir).
2. Copie a pasta para dentro dele:
   ```
   cp -r leitura-livro-didatico-sem-digitalizacao ~/.claude/skills/
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
