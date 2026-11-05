---
name: claude-code-senior
description: Instala 5 ferramentas que melhoram o Claude Code: Agent Skills, Context7, Graphify, 21st Magic e Strix. Use quando pedirem para o Claude Code programar melhor, documentação atualizada, mapa do projeto, componentes prontos ou teste de segurança.
---

# Claude Code programando como sênior

Você instala as ferramentas uma por vez, na ordem, e testa cada uma em uma tarefa real.

## As 5 ferramentas (conferidas em 05/11/2026)
| Passo | Ferramenta | Para que serve | Como instalar |
|---|---|---|---|
| 1 | Agent Skills (github.com/addyosmani/agent-skills, MIT) | Skills do ciclo inteiro: plano, código, teste, revisão | `npx skills add addyosmani/agent-skills -g` |
| 2 | Context7 (github.com/upstash/context7, MIT) | Documentação atualizada de cada biblioteca | `claude mcp add --scope user context7 -- npx -y @upstash/context7-mcp` |
| 3 | Graphify (github.com/Graphify-Labs/graphify, Apache 2.0) | Mapa do projeto inteiro, para gastar menos tokens | Siga o README |
| 4 | 21st Magic (github.com/21st-dev/magic-mcp, ISC) | Componentes de interface prontos | Pede chave grátis em 21st.dev; a pessoa cola no `.env` |
| 5 | Strix (github.com/usestrix/strix, Apache 2.0) | Testa a segurança do app como um hacker | Siga o README. Pede Docker e a chave de um modelo |

## Como conduzir
1. Pergunte a linguagem, o tipo de projeto e o que mais dá errado hoje.
2. Instale a ferramenta que ataca esse problema primeiro.
3. Teste em uma tarefa pequena e mostre o resultado.
4. Só avance com o teste aprovado.

## Regras
- Rode o Strix **apenas no próprio app**, ou em um sistema com autorização escrita. Prefira o ambiente de teste, nunca produção sem aviso.
- Ferramenta de terceiro: antes de instalar, leia o README e confira a licença. Chave e senha ficam só no `.env` da sua máquina, nunca no chat.
- Mais ferramenta consome mais contexto: desligue o que não usar.
