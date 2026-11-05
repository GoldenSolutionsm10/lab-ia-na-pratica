---
name: copiar-estilo-de-reel
description: Analisa um Reel de referência e recria o estilo com Hypit, HyperFrames, Rhubarb e Cutboard. Use quando pedirem para copiar o estilo de um vídeo, analisar um Reel viral ou editar vídeo pelo chat.
---

# Copiar o estilo de um Reel viral com IA

Você ajuda a pessoa a recriar o estilo de um vídeo de referência com conteúdo próprio. Copie a estrutura e o ritmo, nunca a obra.

## As ferramentas (conferidas em 05/11/2026)
| Passo | Ferramenta | Para que serve | Como instalar |
|---|---|---|---|
| 1 | Hypit (github.com/hypit-ai/hypit) | Analisa estilo, animações, cortes e estrutura | `npx skills add hypit-ai/hypit -g` |
| 2 | HyperFrames (github.com/heygen-com/hyperframes) | Animação por código no mesmo estilo | `npx skills add heygen-com/hyperframes` |
| 3 | Rhubarb (github.com/DanielSWolf/rhubarb-lip-sync) | Mexe a boca do personagem junto com o áudio | Baixe a versão pronta no GitHub |
| 4 | Cutboard (github.com/rakesh0x/OpenCardboard) | Edita pelo chat: cortes, legenda e música | Siga o README. É novo: leia o código antes |

## Passo a passo
1. Peça o vídeo de referência e o assunto do vídeo novo.
2. Extraia: duração, tempo de cada corte, fontes, cores, onde entra cada elemento e a estrutura da fala.
3. Mostre essa análise em tabela e peça aprovação.
4. Escreva o roteiro próprio na mesma estrutura.
5. Monte em HyperFrames. Use Rhubarb se houver personagem falando.
6. Compare os dois lado a lado e ajuste o ritmo.

## Regras
- Não reaproveite imagem, música ou trecho do vídeo original.
- Hypit tem licença com condições: uso próprio e para clientes pode; revender não. Leia antes.
- Ferramenta de terceiro: antes de instalar, leia o README e confira a licença. Chave e senha ficam só no `.env` da sua máquina, nunca no chat.
