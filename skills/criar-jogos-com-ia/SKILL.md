---
name: criar-jogos-com-ia
description: Instala e usa o pacote aberto de 77 skills de desenvolvimento de jogos (awesome-gamedev-agent-skills) no Claude Code, para criar jogos em Godot, Unity, Unreal ou para web, do zero até publicar. Use quando pedirem para criar um jogo, instalar as skills de game dev, escolher a engine ou adicionar uma mecânica (pulo, inventário, fase, menu).
---

# Criar jogos com o Claude

Você guia a pessoa pelo pacote **awesome-gamedev-agent-skills** (github.com/gamedev-skills/awesome-gamedev-agent-skills, licença Apache-2.0, conferido em 10/11/2026). São 77 skills de game dev e um "router" que escolhe sozinho a skill certa para a engine e para a tarefa.

## Pré-requisitos
- Claude Code instalado.
- Node.js 22.20 ou mais novo (para o comando `npx`).
- A engine do jogo, se não for para web: Godot, Unity ou Unreal (todas têm versão grátis).

## Instalar (escolha um)
1. **Tudo de uma vez:** `npx skills add gamedev-skills/awesome-gamedev-agent-skills` (coloque `-g` para valer em todos os projetos).
2. **Como plugin do Claude:**
   - `claude plugin marketplace add gamedev-skills/awesome-gamedev-agent-skills`
   - `claude plugin install gamedev@awesome-gamedev-agent-skills`
3. **Só uma engine (mais leve):** `claude plugin install router@awesome-gamedev-agent-skills` e depois `claude plugin install godot@awesome-gamedev-agent-skills` (ou `unity`, `unreal`, `web-engines`).

## Passo a passo
1. Pergunte qual jogo a pessoa quer e em qual engine. Sem engine? Sugira web (Phaser ou three.js) para testar rápido no navegador, ou Godot para jogo 2D grátis.
2. Instale pelo caminho acima e abra uma sessão nova do Claude Code na pasta do jogo.
3. Comece pequeno: uma tela, um personagem andando. Depois uma mecânica por vez (pulo, inimigo, pontuação, menu, salvar).
4. Teste a cada passo e só então peça o próximo.
5. No fim, ajude a exportar o jogo para a plataforma escolhida (web, celular, Steam). Publicar e cobrar pede conta de desenvolvedor de cada loja: isso a pessoa faz.

## Regras
- O pacote é de terceiros: leia o README e a licença antes de usar.
- Arte, música e nomes de jogos famosos têm dono: crie personagens e arte próprios.
- Chave, senha e dados de pagamento das lojas nunca vão no chat.
