# claude-skills-vania

Coleção de skills para o Claude voltadas ao estudo e à análise de textos
acadêmicos, desenvolvidas para uso em contexto de ensino e pesquisa.

## Skills

| Skill | O que faz |
|---|---|
| [`leitura-analitica-severino/`](./leitura-analitica-severino/) | Conduz a leitura analítica de um texto acadêmico e gera um fichamento, seguindo o método de Antônio Joaquim Severino (*Metodologia do Trabalho Científico*). Entrega um documento de análise para consulta posterior. |
| [`tutor-de-texto/`](./tutor-de-texto/) | Conduz uma sessão de estudo interativa e conversacional, ponto a ponto, até que a pessoa consiga explicar o núcleo do artigo com as próprias palavras. Foco no processo de tutoria, não apenas no documento final. |

As duas skills são complementares: `tutor-de-texto` é útil para uma
primeira compreensão guiada do texto, enquanto `leitura-analitica-severino`
produz o registro formal de análise depois que o texto já foi trabalhado
(ou de forma independente, para quem já tem domínio de leitura acadêmica).

## Estrutura do repositório

```
claude-skills-vania/
├── README.md                          # este arquivo
├── LICENSE                            # MIT
├── leitura-analitica-severino/
│   ├── SKILL.md
│   └── README.md
└── tutor-de-texto/
    ├── SKILL.md
    └── README.md
```

Cada skill é independente e pode ser empacotada (`.skill`/`.zip`) e
instalada separadamente a partir da sua própria pasta.

## Instalação

Para usar uma skill no Claude, copie a pasta correspondente (contendo o
`SKILL.md`) para o diretório de skills do usuário, ou gere um pacote
`.skill`/`.zip` a partir dela para distribuição/instalação.

## Licença

MIT — ver [LICENSE](./LICENSE).
