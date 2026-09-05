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

> **Não usa Git/GitHub?** Dá para baixar só esta pasta pelo navegador, sem instalar nada além de um programa de descompactar: acesse
> `https://github.com/vaniago/kit_leitura_academica/tree/main/leitura-livro-didatico-sem-digitalizacao`
> no GitHub, copie o endereço da página, cole em [download-directory.github.io](https://download-directory.github.io) e baixe — o `.zip` gerado já serve direto para o passo 2 da Opção 1 abaixo. (Ou baixe [o kit inteiro](../README.md#antes-de-tudo-baixando-os-arquivos-pelo-navegador-sem-usar-git), que traz esta e as demais skills.)

**Opção 1 — pelo Claude no navegador (claude.ai):**

1. Se você usou `download-directory.github.io` acima, já tem o `.zip` pronto — pule para o passo 2. Senão, compacte a pasta `leitura-livro-didatico-sem-digitalizacao/` (contendo o `SKILL.md`) em um `.zip`:
   - **Windows:** clique com o botão direito na pasta → **Enviar para →
     Pasta compactada** (ou, no PowerShell: `Compress-Archive -Path
     .\leitura-livro-didatico-sem-digitalizacao\* -DestinationPath .\leitura-livro-didatico-sem-digitalizacao.zip`).
   - **macOS:** clique com o botão direito na pasta → **Comprimir**.
   - **Linux / terminal (macOS incluso):**
     ```
     cd leitura-livro-didatico-sem-digitalizacao && zip -r ../leitura-livro-didatico-sem-digitalizacao.zip .
     ```
2. No claude.ai, vá em **Configurações → Habilidades (Capabilities) →
   Adicionar habilidade**.
3. Faça o upload do `.zip` gerado.

**Opção 2 — copiar a pasta direto (Claude Code):**

1. Localize o diretório de skills do usuário: `~/.claude/skills/`
   (Linux/macOS) ou `%USERPROFILE%\.claude\skills\` no Windows — em
   ambos os casos, crie a pasta `skills` se ela ainda não existir.
2. Copie a pasta para dentro dele:
   - **Linux/macOS:**
     ```
     cp -r leitura-livro-didatico-sem-digitalizacao ~/.claude/skills/
     ```
   - **Windows (PowerShell):**
     ```
     New-Item -ItemType Directory -Force -Path "$env:USERPROFILE\.claude\skills" | Out-Null
     Copy-Item -Recurse -Path .\leitura-livro-didatico-sem-digitalizacao -Destination "$env:USERPROFILE\.claude\skills\"
     ```
3. Reinicie o Claude Code (ou abra uma nova sessão) para que a skill seja
   carregada.

**Opção 3 — empacotar como `.skill`/`.zip` para distribuir a terceiros:**

1. Compacte a pasta do mesmo jeito da Opção 1 (no sistema operacional de
   quem estiver empacotando).
2. Compartilhe o arquivo gerado com quem for instalar.
3. Quem receber pode usar tanto a Opção 1 (upload pelo navegador) quanto
   a Opção 2 (pasta de skills local), conforme onde for usar o Claude e
   qual for o sistema operacional — o `.zip` funciona nos dois casos, em
   qualquer sistema.

## Licença

MIT — ver [LICENSE](../LICENSE) na raiz do repositório.
