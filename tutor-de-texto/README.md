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

1. Mapeia os conceitos-chave do texto e organiza uma sequência lógica de
   ensino.
2. Apresenta um mapa breve da jornada de estudo.
3. Explica um conceito por vez, em linguagem acessível, com analogias.
4. Verifica ativamente a compreensão da pessoa antes de avançar — nunca
   pula essa checagem.
5. Reforça pontos com lacuna antes de seguir adiante.
6. Ao final, valida se a pessoa consegue sintetizar tema, problema, tese e
   conclusão do artigo.
7. Gera um arquivo `.md` com o roteiro de estudo da sessão.

Pensada especialmente para quem tem dificuldade de manter atenção em
textos longos, mas é genérica: aplica-se a qualquer artigo, de qualquer
área de conhecimento.

## Instalação

**Opção 1 — pelo Claude no navegador (claude.ai):**

1. Compacte a pasta `tutor-de-texto/` (contendo o `SKILL.md`) em um `.zip`:
   ```
   cd tutor-de-texto && zip -r ../tutor-de-texto.zip .
   ```
2. No claude.ai, vá em **Configurações → Habilidades (Capabilities) →
   Adicionar habilidade**.
3. Faça o upload do `.zip` gerado.

**Opção 2 — copiar a pasta direto (Claude Code):**

1. Localize o diretório de skills do usuário: `~/.claude/skills/` (crie-o
   se ainda não existir).
2. Copie a pasta para dentro dele:
   ```
   cp -r tutor-de-texto ~/.claude/skills/
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
