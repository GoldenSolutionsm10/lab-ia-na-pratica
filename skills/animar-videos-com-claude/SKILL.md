---
name: animar-videos-com-claude
description: Leva um tema do dia a dia até um vídeo animado em código: pesquisa, roteiro, voz, animação, sincronia com a voz e revisão. Use quando pedirem para animar um vídeo explicativo com o Claude, fazer Reels animados sem rosto ou montar a animação no Remotion.
---

# Animar vídeos com o Claude em 5 passos

Você ajuda a pessoa a sair de um tema até um vídeo animado de 30 a 45 segundos, com tudo desenhado em código (sem imagem de banco).

## O que precisa
| Item | Para quê | Custo |
|---|---|---|
| Claude Code (no computador) | Escreve o roteiro, o código da animação e revisa | plano do Claude |
| Remotion (github.com/remotion-dev/remotion) | Vídeo feito em código React | grátis para pessoa física e empresa de até 3 pessoas; leia a licença |
| Uma voz (a sua gravada ou uma de IA) | A narração | depende da ferramenta |
| Whisper (github.com/openai/whisper, MIT) | Tempo de cada palavra da voz, para a sincronia | grátis, roda no computador |

## Passo 1 · Tema
Escolha uma coisa que todo mundo usa todo dia e ninguém sabe como funciona. Peça 10 opções e fique com a que tem uma pergunta curiosa (ex.: "deixar o notebook sempre na tomada acaba com a bateria?").

## Passo 2 · Pesquisa, roteiro, voz e legenda
1. Pesquise 3 fontes confiáveis e anote a resposta com a fonte.
2. Roteiro de 30 a 45 s: gancho com a pergunta (1ª frase), 3 a 4 frases de explicação, fechamento com chamada.
3. Grave ou gere a voz. Rode o Whisper com tempo por palavra e guarde o `palavras.json`.

## Passo 3 · Desenhar em código
Crie um projeto Remotion (`npx create-video@latest`). Uma cena por frase do roteiro. Formas, ícones e texto feitos em código. Vertical 1080x1920, 30 quadros por segundo.

## Passo 4 · Casar a animação com a voz
Use o `palavras.json`: cada objeto entra no quadro em que a palavra é falada (`quadro = segundos x 30`). Quando a voz diz "bateria", a bateria aparece.

## Passo 5 · Revisar e consertar
Renderize, tire um quadro a cada 2 s numa folha (grade de imagens) e confira: texto cortado, objeto fora da tela, cena parada mais de 1,5 s. Conserte e renderize de novo.

## Regras
- Dado só com fonte. Não invente número.
- Nada de marca, personagem ou logo de terceiros sem licença.
- Vídeo com voz de IA: marque "conteúdo gerado por IA" na rede social.

Também quer usar IA no atendimento? Veja a skill `guia-ia-no-atendimento` neste mesmo repositório.
