# tutor-de-texto

Skill para o Claude que conduz uma sessão de estudo interativa e
conversacional sobre um artigo acadêmico ou técnico, ponto a ponto, até que
a pessoa consiga explicar o núcleo do texto com as próprias palavras.

## O que faz

Diferente de um fichamento (que produz um documento de análise para
consulta posterior), esta skill foca no **processo** de tutoria:

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

Copie a pasta `tutor-de-texto/` (contendo `SKILL.md`) para o diretório de
skills do usuário do Claude, ou instale a partir do pacote `.skill`/`.zip`
gerado a partir desta pasta.

## Licença

MIT — ver [LICENSE](../LICENSE) na raiz do repositório.
