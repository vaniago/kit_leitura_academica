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

Pensada especialmente para alunos de ensino técnico ou médio, alunos de
início de graduação, ou qualquer pessoa leiga no assunto do texto mas que
já lê e compreende texto normalmente.

## Instalação

Copie a pasta `leitura-guiada/` (contendo `SKILL.md`) para o diretório de
skills do usuário do Claude, ou instale a partir do pacote `.skill`/`.zip`
gerado a partir desta pasta.

## Licença

MIT — ver [LICENSE](../LICENSE) na raiz do repositório.
