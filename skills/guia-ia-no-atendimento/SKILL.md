---
name: guia-ia-no-atendimento
description: Mostra onde um profissional usa IA hoje e onde falta usar, e monta o atendimento no WhatsApp com resumo antes da call. Use quando pedirem um guia para usar IA no escritório, ir além da petição ou organizar o contato com o cliente.
---

# Usar IA além de escrever: o atendimento

Você mostra à pessoa o que ela já faz com IA e o que está sobrando na mão, e ajuda a atacar o atendimento primeiro.

## Passo 1: o mapa
Pergunte em quais tarefas ela usa IA hoje e preencha:
| Tarefa | Usa IA? | Horas por semana | Quem espera por isso |
|---|---|---|---|
| Escrever peças e documentos | | | |
| Pesquisa | | | |
| Responder cliente novo | | | |
| Dar andamento a cliente atual | | | |
| Marcar e confirmar reunião | | | |

## Passo 2: o que atacar
Escolha a linha com mais horas e com alguém esperando do outro lado. Normalmente é o atendimento: o cliente chama no WhatsApp à noite, e quem responde primeiro sai na frente.

## Passo 3: a montagem
1. **Resposta rápida:** agente responde, entende o pedido e marca. Ver a skill `atendente-24h-whatsapp`.
2. **Resumo antes da call:** o profissional recebe quem é, o que pediu, documentos e dúvidas.
3. **Depois da call:** o agente envia os próximos passos, com a aprovação do profissional.

## Modelo do resumo
```
Cliente: <nome> | Chegou por: <canal>
Assunto: <uma frase>
O que ele já contou: <3 itens>
Documentos: <lista>
Urgência: <sim ou não, e por quê>
Perguntas para a call: <3>
```

## Regras
- Comece por uma linha do mapa. Meça as horas antes e depois.
- Texto gerado é rascunho: quem assina revisa.
- Modelo grátis nunca recebe dado de cliente.
