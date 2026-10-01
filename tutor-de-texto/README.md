# tutor-de-texto

Skill para o Claude que conduz uma sessão de estudo interativa e
conversacional sobre um artigo acadêmico ou técnico, ponto a ponto, até que
a pessoa consiga explicar o núcleo do texto com as próprias palavras.

## O que faz

Diferente do `leitura-analitica-severino` (que produz um documento formal
de análise) e do `leitura-guiada` (que acompanha a ordem original do
texto, centrado no leitor, sem reorganizar o conteúdo), esta skill foca
no **processo** de tutoria, reorganizando o conteúdo numa sequência
pedagógica própria:

1. Sugere uma leitura panorâmica inicial do texto inteiro (opcional,
   rápida, sem exigir compreensão) para dar uma visão geral antes de
   começar.
2. Mapeia os conceitos-chave do texto (um por ideia, não por seção —
   seções densas viram vários pontos) e organiza uma sequência lógica de
   ensino, priorizando cobrir todos os aspectos relevantes mesmo que isso
   alongue a sessão.
3. Apresenta um mapa breve da jornada de estudo.
4. Explica um conceito por vez, em linguagem acessível, com analogias —
   no ritmo do leitor, nunca com pressa de avançar. Verifica antes se o
   artigo está desatualizado (dados, classificações, leis, teorias) e
   sinaliza as atualizações em notas curtas, separadas do que o texto
   diz; avisa antes de trechos sensíveis (ex.: suicídio).
5. Verifica ativamente a compreensão da pessoa antes de avançar — nunca
   pula essa checagem, e só a faz depois de ter explicado o conceito por
   inteiro.
6. Reforça pontos com lacuna antes de seguir adiante. Discordâncias
   fundamentadas são tratadas como debate (a skill não concede só para
   avançar), não como lacuna, e ficam registradas no relatório como
   contribuição da pessoa, útil para seminários e debates.
7. Antes de encerrar, oferece uma releitura panorâmica final (opcional)
   e pergunta diretamente se restam dúvidas, esclarecendo-as antes de
   seguir.
8. Valida se a pessoa consegue sintetizar tema, problema, tese e
   conclusão do artigo.
9. Gera um arquivo `.md` com o roteiro de estudo da sessão, registrando
   à parte qualquer lacuna que a própria pessoa teve que apontar (em vez
   de confundir isso com um simples reforço por dificuldade de
   compreensão), as dúvidas levantadas no fechamento, a tabela de
   atualidade do artigo e as questões abertas. Se a pessoa pedir para
   pausar, gera na hora um roteiro parcial para retomar depois.

Pensada especialmente para quem tem dificuldade de manter atenção em
textos longos, mas é genérica: aplica-se a qualquer artigo, de qualquer
área de conhecimento.

## Instalação

> **Não usa Git/GitHub?** Dá para baixar só esta pasta pelo navegador, sem instalar nada além de um programa de descompactar: acesse
> `https://github.com/vaniago/kit_leitura_academica/tree/main/tutor-de-texto`
> no GitHub, copie o endereço da página, cole em [download-directory.github.io](https://download-directory.github.io) e baixe — o `.zip` gerado já serve direto para o passo 2 da Opção 1 abaixo. (Ou baixe [o kit inteiro](../README.md#antes-de-tudo-baixando-os-arquivos-pelo-navegador-sem-usar-git), que traz esta e as demais skills.)

**Opção 1 — pelo Claude no navegador (claude.ai):**

1. Se você usou `download-directory.github.io` acima, já tem o `.zip` pronto — pule para o passo 2. Senão, compacte a pasta `tutor-de-texto/` (contendo o `SKILL.md`) em um `.zip`:
   - **Windows:** clique com o botão direito na pasta → **Enviar para →
     Pasta compactada** (ou, no PowerShell: `Compress-Archive -Path
     .\tutor-de-texto\* -DestinationPath .\tutor-de-texto.zip`).
   - **macOS:** clique com o botão direito na pasta → **Comprimir**.
   - **Linux / terminal (macOS incluso):**
     ```
     cd tutor-de-texto && zip -r ../tutor-de-texto.zip .
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
     cp -r tutor-de-texto ~/.claude/skills/
     ```
   - **Windows (PowerShell):**
     ```
     New-Item -ItemType Directory -Force -Path "$env:USERPROFILE\.claude\skills" | Out-Null
     Copy-Item -Recurse -Path .\tutor-de-texto -Destination "$env:USERPROFILE\.claude\skills\"
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
