# BellaOS — regras para o Claude Code

Este repositório monta a imagem do sistema BellaOS com BlueBuild (`recipes/recipe.yml`).
O planejamento completo (filosofia, decisões, recursos) fica no Notion do projeto.

## Antes de mudar qualquer coisa
- Leia `recipes/recipe.yml` e entenda o que cada módulo faz.
- Mudanças grandes viram proposta escrita antes de virar código.

## Código
- Código legível para humanos: nomes claros, comentários onde não for óbvio.
- Nada entra sem o autor ter lido e entendido. Explique o que mudou e por quê.
- Scripts em `files/scripts/` com `set -euo pipefail` e comentários.
- Nunca coloque segredos no repositório (ex.: `cosign.key`). Só a chave pública `cosign.pub` fica aqui.

## Base e camadas
- Base: Fedora Kinoite oficial. Não manter kernel nem bibliotecas próprias.
- Apps gráficos: Flatpak. Pacotes de outras distros: segunda home (distrobox).
- RPM na imagem só quando precisa de acesso ao sistema (drivers, serviços).

## Uso de IA
- O uso de IA é declarado em `AI_USAGE.md` (atualize a tabela quando uma parte nova usar IA). Commits não levam a linha Co-Authored-By.
- Toda mudança de visual/design é registrada em `DESIGN_LOG.md` (referência, opções, o que o autor escolheu).
- Arte (logo, mascote) é feita pelo autor, não pela IA.
