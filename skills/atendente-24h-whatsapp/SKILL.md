---
name: atendente-24h-whatsapp
description: Cria um agente de atendimento no WhatsApp que responde em segundos, entende o caso e marca a conversa na agenda. Use quando pedirem atendente de IA, responder cliente fora do horário, agendar pelo WhatsApp ou um agente como a Luna.
---

# Atendente de IA que responde à meia-noite

Você monta um agente de atendimento para o primeiro contato: responde rápido, entende o caso e marca a conversa. Ele não resolve o caso.

## Ficha do agente (preencha com a pessoa)
| Item | Exemplo |
|---|---|
| Nome e tom | Luna, acolhedora, frases curtas |
| O que atende | Áreas, serviços, região, horários |
| Perguntas de triagem | No máximo 3, uma por mensagem |
| Quando marca | Caso dentro do escopo: oferece 2 horários reais |
| Quando chama um humano | Urgência, cliente irritado, pedido de preço fora da tabela |
| O que nunca faz | Dar parecer, prometer resultado, inventar informação |

## Fluxo
1. Cumprimenta em segundos e pergunta como pode ajudar.
2. Faz a triagem, uma pergunta por vez.
3. Confere a agenda **por script**, nunca de cabeça.
4. Oferece 2 horários e confirma.
5. Envia ao profissional um resumo: quem é, o que precisa, urgência.

## Como construir
1. Escreva a ficha.
2. Crie uma lista com 20 conversas de teste, incluindo as difíceis.
3. Ligue o agente a um número de WhatsApp dedicado e à agenda.
4. Rode em teste, com a pessoa fazendo o papel do cliente.
5. Ligue para clientes reais por uma semana, com a pessoa lendo as conversas.

## Regras
- Se perguntarem, ele diz que é assistente virtual.
- Sem envio em massa. Ele responde a quem chamou.
- Dados pessoais só o necessário, e proteja-os conforme a LGPD.
- Modelo grátis nunca recebe dado de cliente.
