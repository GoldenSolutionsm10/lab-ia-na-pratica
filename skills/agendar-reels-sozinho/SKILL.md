---
name: agendar-reels-sozinho
description: Monta uma fila que publica os seus Reels sozinha no horário marcado, num servidor seu, e liga cada vídeo à palavra do comentário que entrega o material no direct. Use quando pedirem para agendar Reels, deixar a semana postando sozinha ou organizar legenda, palavra e material de cada vídeo.
---

# Agendar a semana de Reels sozinho

Você monta com a pessoa uma semana de Reels que publica sozinha. Cada vídeo sai com legenda, palavra no comentário e material pronto para quem comentar.

## Pergunte antes
1. Quantos Reels por dia e em quais horários?
2. Onde ficam os vídeos?
3. Tem servidor (VPS) e acesso à API do Instagram (conta profissional, app da Meta ou um conector)?
4. Usa automação de comentário para direct?

## Para cada Reel, um passo só
| # | O quê | Pronto quando |
|---|---|---|
| 1 | Ler ou ouvir o que o vídeo fala | Sei a palavra e o que ela promete |
| 2 | Legenda | 1ª frase curta sobre o vídeo, chamada com a palavra, 3 hashtags, nenhum número que o vídeo não diz |
| 3 | Material da palavra | Página, arquivo ou repositório no ar antes do post |
| 4 | Palavra na automação | Palavra e erros de digitação cadastrados |
| 5 | Fila | Item com data, hora, arquivo, legenda e quadro da capa |

## A fila (script, sem IA)
- Um arquivo `fila.json` com os itens, e os vídeos no servidor.
- Um script roda a cada 5 minutos pelo cron e publica o que já passou da hora.
- Publica um por vez e marca como publicado, para nunca sair duas vezes.
- Item muito atrasado não sai sozinho: avisa a pessoa.
- Só roda com um arquivo de liga e desliga, criado depois da aprovação.
- Teste primeiro com um publicador falso, que só grava "publicado".

## Capa
Vídeo com contador começa zerado. Tire quadros em 3, 6 e 10 segundos e escolha o que tem a informação cheia.

## Organização para a pessoa
Uma pasta por dia com os vídeos daquele dia, com hora e palavra no nome, e um arquivo com as legendas.

## Regras
- Nada vai ao ar sem o "sim" da pessoa para a semana.
- Postou à mão? Tire o item da fila.
- Chave e senha só no `.env` do servidor, nunca no chat.
- Reels de teste do Instagram pedem conta com mais público: em conta nova, a API recusa.
