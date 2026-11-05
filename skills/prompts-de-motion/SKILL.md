---
name: prompts-de-motion
description: Usa a biblioteca Prompt Motion para achar um vídeo animado feito com Claude, copiar o prompt e adaptar para a marca da pessoa. Use quando pedirem vídeo animado com Claude, motion de produto, vídeo de lançamento, gráfico animado ou prompts de motion.
---

# Prompts de motion com o Prompt Motion

Você ajuda a pessoa a partir de um vídeo pronto da biblioteca e chegar a um vídeo com a marca dela.

## A biblioteca
https://prompt-motion.com/ reúne vídeos animados feitos com Claude, com o prompt ou a skill de cada um. Há filtros como Product UI, Phone, Charts, Diagrams, Kinetic type e Characters.

## Passo a passo
1. Pergunte o que o vídeo precisa mostrar, a duração e o formato (vertical 9:16 para Reels).
2. Peça à pessoa o link do vídeo que ela curtiu e o prompt copiado da página.
3. Peça os dados da marca: cores, fonte, logo e o texto de cada cena.
4. Adapte o prompt: troque marca, textos e proporção. Mantenha o que dá o estilo: ritmo, transições e efeitos.
5. Rode no Claude Code com um motor de vídeo em código (Remotion ou HyperFrames).
6. Mostre uma folha de quadros, ajuste e só então renderize.

## Exemplo de adaptação
```
Use este prompt como base de estilo: <PROMPT COPIADO>.
Troque a marca por <MARCA>, com as cores <CORES> e a fonte <FONTE>.
Formato vertical 1080x1920. Duração de <N> segundos.
Cenas: 1) <TEXTO> 2) <TEXTO> 3) <TEXTO>.
Mantenha o ritmo, as transições e os efeitos sonoros do original.
```

## Regras
- O prompt é do autor: respeite o que a página disser sobre uso e dê o crédito quando publicar.
- Não copie logo ou marca de terceiros.
- Vídeo curto primeiro: 10 segundos para validar o estilo.
