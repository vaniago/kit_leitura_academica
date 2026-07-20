# leitura-cientifica-keshav

Skill para o Claude que acompanha a leitura de um artigo científico usando
o método das três passadas de S. Keshav.

[KeSHAV, S.*How to Read a Paper*, ACM SIGCOMM Computer Communication Review, 2007.](https://dl.acm.org/doi/epdf/10.1145/1273445.1273458)

## A quem se destina

Proposta para quem precisa ler artigos científicos com
regularidade — estudantes de pós-graduação, pesquisadores, participantes
de grupo de pesquisa — mas serve também para quem está
começando a ler papers pela primeira vez, com a terceira passada
calibrada para não exigir demais de quem ainda não tem prática.

## Escopo

Cobre sempre um único artigo por sessão — não é uma skill de revisão de
literatura (comparar vários artigos de uma área).

## O que faz

Esta skill é específica para artigo/paper científico e estrutura a sessão
em três releituras sucessivas do mesmo texto, cada uma mais profunda que a
anterior:

1. Levanta o motivo da leitura e o nível de experiência da pessoa com
   artigos científicos e com o tema específico — esse nível calibra a
   exigência da terceira passada.
2. **Passada 1 (panorama):** título, resumo, introdução, títulos de seção,
   conclusão e uma olhada nas referências; a pessoa responde os "5 Cs"
   (Categoria, Contexto, Corretude, Contribuições, Clareza).
3. **Passada 2 (compreensão do conteúdo):** leitura mais atenta, com foco
   em figuras/gráficos/tabelas (onde problemas de metodologia costumam
   aparecer) e no argumento central com evidência de apoio.
4. **Passada 3 (leitura crítica):** calibrada pelo nível declarado — de
   identificar suposições e limitações (iniciante) até tentar reconstruir
   o artigo inteiro de memória e apontar pontos fortes e fracos reais
   (avançado/pesquisador).
5. Gera um relatório `.md` da sessão, com o que a pessoa respondeu em cada
   passada — nunca um resumo do artigo escrito pelo Claude.

O princípio central é que **cada passada é feita pela própria pessoa**: o
Claude explica o que observar em cada uma e confere o relato contra o
texto real, mas nunca lê o artigo e entrega um resumo pronto no lugar de
quem está estudando.

## Instalação

Esta skill funciona sozinha — não depende de nenhuma outra skill do kit
estar instalada. Ainda assim, ela faz parte de um conjunto de seis skills
de leitura pensadas para situações diferentes (veja o
[README do kit](../README.md)); se você lida com mais de um tipo de texto
(artigo científico, obra literária, livro didático sem digitalização
etc.), pode valer a pena instalar o kit completo em vez de só esta pasta,
para poder trocar de skill caso uma não esteja rendendo numa sessão
específica.

**Opção 1 — pelo Claude no navegador (claude.ai):**

1. Compacte a pasta `leitura-cientifica-keshav/` (contendo o `SKILL.md`)
   em um `.zip`:
   ```
   cd leitura-cientifica-keshav && zip -r ../leitura-cientifica-keshav.zip .
   ```
2. No claude.ai, vá em **Configurações → Habilidades (Capabilities) →
   Adicionar habilidade**.
3. Faça o upload do `.zip` gerado.

**Opção 2 — copiar a pasta direto (Claude Code):**

1. Localize o diretório de skills do usuário: `~/.claude/skills/` (crie-o
   se ainda não existir).
2. Copie a pasta para dentro dele:
   ```
   cp -r leitura-cientifica-keshav ~/.claude/skills/
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
