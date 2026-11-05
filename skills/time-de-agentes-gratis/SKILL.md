---
name: time-de-agentes-gratis
description: Instala e combina 5 repositórios abertos para rodar um time de agentes de IA (Orca, Paperclip, Hindsight, AX e Agent Substrate). Use quando pedirem para rodar vários agentes juntos, montar uma empresa de agentes ou dar memória a um agente.
---

# Time de agentes de graça em 5 passos

Você ajuda a pessoa a montar um time de agentes com repositórios abertos, um passo por vez. Não instale tudo de uma vez.

## Os 5 repositórios (conferidos em 05/11/2026)
| Passo | Ferramenta | Para que serve | Repositório | Licença |
|---|---|---|---|---|
| 1 | Orca | Roda Claude Code, Codex e outros lado a lado e avisa quando cada um termina | github.com/stablyai/orca | MIT |
| 2 | Paperclip | Monta uma empresa de agentes, com cargos, em um painel só | github.com/paperclipai/paperclip | MIT |
| 3 | Hindsight | Memória para os agentes, que aprende com o tempo | github.com/vectorize-io/hindsight | MIT |
| 4 | AX (Google) | Roda muitos agentes ao mesmo tempo | github.com/google/ax | Apache 2.0 |
| 5 | Agent Substrate | Cada agente em um ambiente isolado: se um quebra, os outros seguem | github.com/agent-substrate/substrate | Apache 2.0 |

## Como conduzir
1. Pergunte o que o time vai fazer e em que máquina vai rodar.
2. Comece pelo Orca. Para a maioria, ele basta nos primeiros dias.
3. Para cada repositório: leia o README atual, explique em 2 linhas, instale e teste com uma tarefa pequena.
4. Só avance quando o passo anterior estiver funcionando.
5. AX e Substrate são para quem já roda muitos agentes. Se a pessoa roda 2 ou 3, diga que não precisa deles agora.

## Regras
- Ferramenta de terceiro: antes de instalar, leia o README e confira a licença. Chave e senha ficam só no `.env` da sua máquina, nunca no chat.
- Cada agente recebe só o acesso de que precisa.
- Agente que envia mensagem, publica ou gasta dinheiro pede aprovação humana.
