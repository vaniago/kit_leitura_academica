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

> **Não usa Git/GitHub?** Dá para baixar só esta pasta pelo navegador, sem instalar nada além de um programa de descompactar: acesse
> `https://github.com/vaniago/kit_leitura_academica/tree/main/leitura-guiada`
> no GitHub, copie o endereço da página, cole em [download-directory.github.io](https://download-directory.github.io) e baixe — o `.zip` gerado já serve direto para o passo 2 da Opção 1 abaixo. (Ou baixe [o kit inteiro](../README.md#antes-de-tudo-baixando-os-arquivos-pelo-navegador-sem-usar-git), que traz esta e as demais skills.)

**Opção 1 — pelo Claude no navegador (claude.ai):**

1. Se você usou `download-directory.github.io` acima, já tem o `.zip` pronto — pule para o passo 2. Senão, compacte a pasta `leitura-guiada/` (contendo o `SKILL.md`) em um `.zip`:
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
2. Copie a pasta para dentro dele:
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

1. Compacte a pasta do mesmo jeito da Opção 1 (no sistema operacional de
   quem estiver empacotando).
2. Compartilhe o arquivo gerado com quem for instalar.
3. Quem receber pode usar tanto a Opção 1 (upload pelo navegador) quanto
   a Opção 2 (pasta de skills local), conforme onde for usar o Claude e
   qual for o sistema operacional — o `.zip` funciona nos dois casos, em
   qualquer sistema.

## Licença

MIT — ver [LICENSE](../LICENSE) na raiz do repositório.
