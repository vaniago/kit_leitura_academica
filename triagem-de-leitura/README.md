# triagem-de-leitura

Skill para o Claude que ajuda a pessoa a escolher, entre as demais skills
deste kit, qual encaixa melhor com o texto que ela tem em mãos e o
objetivo da leitura.

## A quem se destina

Para quem tem um texto para estudar mas não sabe qual das seis skills de
leitura do kit usar — ou quer entender rapidamente a diferença entre
elas antes de decidir.

## O que faz

Não conduz nenhuma etapa de leitura, análise ou fichamento — só faz uma
triagem breve, pergunta a pergunta:

1. Se apresenta como consultor de escolha de skill e explica, em poucas
   frases, a finalidade de cada uma das seis skills de leitura do kit.
2. Pergunta que tipo de texto é (artigo científico, obra literária,
   capítulo de livro didático, ou outro texto acadêmico/técnico) e em que
   meio ele está (digitalizado ou só em papel).
3. Pergunta o quanto a pessoa já tem prática lendo esse tipo de texto por
   conta própria — essa resposta pesa na recomendação mesmo quando o tipo
   de texto aponta "naturalmente" para uma única skill (ex.: um artigo
   científico não vai automaticamente para `leitura-cientifica-keshav` se
   a pessoa nunca leu nada parecido sozinha; `tutor-de-texto` pode entrar
   como caminho inicial).
4. Para texto acadêmico/técnico genérico, pergunta também o objetivo
   principal da leitura (documento de análise formal, garantir
   compreensão real do núcleo do texto, ou acompanhamento na própria
   ordem do texto).
5. Apresenta as opções relevantes para o caso (não a lista inteira das
   sete skills, só as que fazem sentido) e diz qual delas recomenda, com
   justificativa breve.
6. Confirma com a pessoa qual ela quer usar e encaminha — seguindo direto
   com a skill escolhida se ela estiver disponível, ou orientando a
   instalação a partir do [README do kit](../README.md) se não estiver.

Se a pessoa já sabe qual skill quer (já nomeou o método, o autor de
referência ou o tipo de texto com clareza), esta skill não deve ser
acionada — a triagem existe só para o caso de indecisão real.

## Instalação

> **Não usa Git/GitHub?** Dá para baixar só esta pasta pelo navegador, sem instalar nada além de um programa de descompactar: acesse
> `https://github.com/vaniago/kit_leitura_academica/tree/main/triagem-de-leitura`
> no GitHub, copie o endereço da página, cole em [download-directory.github.io](https://download-directory.github.io) e baixe — o `.zip` gerado já serve direto para o passo 2 da Opção 1 abaixo. (Ou baixe [o kit inteiro](../README.md#antes-de-tudo-baixando-os-arquivos-pelo-navegador-sem-usar-git), que traz esta e as demais skills.)

**Opção 1 — pelo Claude no navegador (claude.ai):**

1. Se você usou `download-directory.github.io` acima, já tem o `.zip` pronto — pule para o passo 2. Senão, compacte a pasta `triagem-de-leitura/` (contendo o `SKILL.md`) em um `.zip`:
   - **Windows:** clique com o botão direito na pasta → **Enviar para →
     Pasta compactada** (ou, no PowerShell: `Compress-Archive -Path
     .\triagem-de-leitura\* -DestinationPath .\triagem-de-leitura.zip`).
   - **macOS:** clique com o botão direito na pasta → **Comprimir**.
   - **Linux / terminal (macOS incluso):**
     ```
     cd triagem-de-leitura && zip -r ../triagem-de-leitura.zip .
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
     cp -r triagem-de-leitura ~/.claude/skills/
     ```
   - **Windows (PowerShell):**
     ```
     New-Item -ItemType Directory -Force -Path "$env:USERPROFILE\.claude\skills" | Out-Null
     Copy-Item -Recurse -Path .\triagem-de-leitura -Destination "$env:USERPROFILE\.claude\skills\"
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
