# leitura-analitica-severino

Skill para o Claude que conduz a leitura analítica de um texto acadêmico e
gera um fichamento, seguindo o roteiro de Antônio Joaquim Severino em
*Metodologia do Trabalho Científico* (SEVERINO, 2017).

## O que faz

Conduz internamente as cinco etapas do método (análise textual, análise
temática, análise interpretativa, problematização e síntese pessoal) e
entrega o resultado em um dos seis formatos de saída:

- Fichamento bibliográfico
- Fichamento de citações
- Resumo indicativo (NBR 6028)
- Resumo informativo (NBR 6028)
- Resenha completa / resumo crítico (NBR 6028)
- Fichamento analítico integral (formato padrão)

Também pode gerar, como entregável opcional, um mapa conceitual em formato
de importação do CmapTools.

O CmapTools está disponível [aqui](https://cmap.ihmc.us/)

## Instalação

**Opção 1 — pelo Claude no navegador (claude.ai):**

1. Compacte a pasta `leitura-analitica-severino/` (contendo o `SKILL.md`)
   em um `.zip`:
   ```
   cd leitura-analitica-severino && zip -r ../leitura-analitica-severino.zip .
   ```
2. No claude.ai, vá em **Configurações → Habilidades (Capabilities) →
   Adicionar habilidade**.
3. Faça o upload do `.zip` gerado.

**Opção 2 — copiar a pasta direto (Claude Code):**

1. Localize o diretório de skills do usuário: `~/.claude/skills/` (crie-o
   se ainda não existir).
2. Copie a pasta para dentro dele:
   ```
   cp -r leitura-analitica-severino ~/.claude/skills/
   ```
3. Reinicie o Claude Code (ou abra uma nova sessão) para que a skill seja
   carregada.

**Opção 3 — empacotar como `.skill`/`.zip` para distribuir a terceiros:**

1. Compacte a pasta do mesmo jeito da Opção 1.
2. Compartilhe o arquivo gerado com quem for instalar.
3. Quem receber pode usar tanto a Opção 1 (upload pelo navegador) quanto
   a Opção 2 (`~/.claude/skills/`), conforme onde for usar o Claude.

## Referência

SEVERINO, Antônio Joaquim. *Metodologia do trabalho científico*. 24. ed.
rev. e ampl. São Paulo: Cortez, 2017.

## Licença

MIT — ver [LICENSE](../LICENSE) na raiz do repositório.
