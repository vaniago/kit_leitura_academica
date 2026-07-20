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

1. Pergunta que tipo de texto é (artigo científico, obra literária,
   capítulo de livro didático sem digitalização, ou outro texto
   acadêmico/técnico já digitalizado).
2. Para texto acadêmico/técnico genérico, pergunta o objetivo principal
   da leitura (documento de análise formal, garantir compreensão real do
   núcleo do texto, ou acompanhamento na própria ordem do texto).
3. Recomenda a skill correspondente com uma justificativa breve, confirma
   com a pessoa, e encaminha — seguindo direto com a skill recomendada se
   ela estiver disponível, ou orientando a instalação a partir do
   [README do kit](../README.md) se não estiver.

Se a pessoa já sabe qual skill quer (já nomeou o método, o autor de
referência ou o tipo de texto com clareza), esta skill não deve ser
acionada — a triagem existe só para o caso de indecisão real.

## Instalação

**Opção 1 — pelo Claude no navegador (claude.ai):**

1. Compacte a pasta `triagem-de-leitura/` (contendo o `SKILL.md`) em um
   `.zip`:
   ```
   cd triagem-de-leitura && zip -r ../triagem-de-leitura.zip .
   ```
2. No claude.ai, vá em **Configurações → Habilidades (Capabilities) →
   Adicionar habilidade**.
3. Faça o upload do `.zip` gerado.

**Opção 2 — copiar a pasta direto (Claude Code):**

1. Localize o diretório de skills do usuário: `~/.claude/skills/` (crie-o
   se ainda não existir).
2. Copie a pasta para dentro dele:
   ```
   cp -r triagem-de-leitura ~/.claude/skills/
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
