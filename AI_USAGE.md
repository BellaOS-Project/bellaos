# Uso de IA na BellaOS

A BellaOS é um projeto feito por uma pessoa com ajuda de IA. Este arquivo existe para deixar claro onde a IA entrou e onde não entrou.

## Quem decide

A ideia, a identidade, a arquitetura e a decisão do que entra no sistema são do autor (Richard Spinola). A IA é uma ferramenta: ela escreve código e sugere caminhos, e o autor revisa, entende e aprova antes de qualquer coisa entrar.

## Onde a IA foi usada

| Parte | IA usada | Como |
|---|---|---|
| Planejamento inicial | Claude, Gemini | Conversas para levantar problemas do Linux, comparar bases e organizar as decisões. As decisões finais são do autor. |
| Receita da imagem (`recipes/recipe.yml`) | Claude (Claude Code) | Configuração inicial sobre o Fedora Kinoite. |
| Regras para IA (`CLAUDE.md`) | Claude | Escrito a partir das regras definidas pelo autor. |

Esta tabela é atualizada sempre que uma parte nova do projeto usar IA.

## Onde a IA não é usada

- Arte: logo, mascote e identidade visual são feitos pelo autor.
- Sugestões de design vindas de IA, quando existirem, são registradas em `DESIGN_LOG.md`.

## Regras

- Nenhum código entra sem o autor ter lido e entendido.
- Tudo que mexe com sistema ou senha passa por revisão de segurança.
- O código é escrito para ser legível por humanos, para que qualquer pessoa consiga manter o projeto sem depender de uma IA específica.
