---
name: plugins-do-claude
description: Instala os 5 plugins do Reel (FreeLLMAPI, Agent Reach, SkillSpector, Lemo Opuscar e Ponytail) e os plugins oficiais de trabalho da Anthropic (vendas, marketing, jurídico, financeiro e outros). Use quando pedirem plugins para o Claude Code ou para montar um time de especialistas no Claude.
---

# Plugins para o Claude: os 5 do Reel e a loja oficial

Você instala plugins no Claude Code, um por vez, e testa cada um. Pergunte primeiro o que a pessoa quer resolver.

## Os 5 plugins do Reel (conferidos em 05/11/2026)
| # | Plugin | Para que serve | Como instalar |
|---|---|---|---|
| 1 | FreeLLMAPI (github.com/tashfeenahmed/freellmapi, MIT) | Junta provedores gratuitos em um endereço só e troca sozinho quando um estoura | `curl -fsSL https://freellmapi.co/install.sh \| bash` (pede Docker; leia o script antes) |
| 2 | Agent Reach (github.com/Panniantong/Agent-Reach, MIT) | Deixa o agente ler e pesquisar em Reddit, YouTube, Twitter e GitHub | Peça ao Claude para seguir `docs/install.md` do repositório. O pacote de mesmo nome no PyPI não é deste projeto |
| 3 | SkillSpector (github.com/NVIDIA/SkillSpector, Apache 2.0) | Procura código malicioso em uma skill antes de instalar | `uv tool install git+https://github.com/NVIDIA/skillspector.git`, depois `skillspector scan ./a-skill/` |
| 4 | Lemo Opuscar (github.com/lemomo-ai/lemo-opuscar, MIT) | Ensina o Claude a animar vídeo em dezenas de estilos | `claude plugin marketplace add lemomo-ai/lemo-opuscar` e `claude plugin install lemo-opuscar@lemolab` |
| 5 | Ponytail (github.com/DietrichGebert/ponytail, MIT) | Faz o agente escrever menos código e gastar menos tokens | `/plugin marketplace add DietrichGebert/ponytail` e `/plugin install ponytail@ponytail` |

Instale o SkillSpector primeiro e use-o para checar as skills seguintes.

## A loja oficial da Anthropic
Repositório: github.com/anthropics/knowledge-work-plugins (Apache 2.0). Áreas como vendas, marketing, jurídico, financeiro, dados, RH e operações.
1. `claude plugin marketplace add anthropics/knowledge-work-plugins`
2. `claude plugin install sales@knowledge-work-plugins` (troque `sales` por `marketing`, `legal`, `finance`...)
3. Use: `/sales:call-prep com o cliente X`

Saída do plugin jurídico é rascunho: um advogado revisa antes de usar.

## Regras
- Ferramenta de terceiro: antes de instalar, leia o README e confira a licença. Chave e senha ficam só no `.env` da sua máquina, nunca no chat.
- Provedor gratuito pode usar o que você envia: não mande dado de cliente por ele.
- Depois de instalar, faça um teste pequeno e diga o que funcionou.
