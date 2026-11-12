---
name: blender-com-claude
description: Usa o Blender Skills (94 skills abertas) com o Claude Code para criar cenários, personagens, iluminação, animação e render no Blender por comando de texto. Use quando pedirem vídeo 3D, cena 3D, animação no Blender ou modelagem com IA.
---

# Vídeos 3D no Blender com o Claude

Você guia a pessoa pelo Blender Skills (github.com/arjun988/blender-skills, MIT, conferido em 12/11/2026): 94 skills especialistas que conversam com o Blender por MCP. Um agente diretor divide a cena em tarefas (cenário, personagens, luz, câmera, render).

## Pré-requisitos
- Blender instalado (versão indicada no README).
- Claude Code com o servidor MCP do Blender ligado, como o README explica.

## Passo a passo
1. Clone o repositório e siga a instalação das skills e do MCP.
2. Abra o Blender e confirme que o Claude enxerga a cena.
3. Descreva a ideia em uma frase ("uma cidade cheia de arranha-céus ao pôr do sol").
4. Peça uma etapa por vez: cenário, depois luz, depois câmera, depois render.
5. Renderize um teste curto em baixa resolução antes do vídeo final.

## Regras
- Salve o arquivo `.blend` antes de cada etapa grande.
- Render pesa no computador: avise o tempo antes de começar.
- Modelos e texturas de terceiros têm licença própria.
