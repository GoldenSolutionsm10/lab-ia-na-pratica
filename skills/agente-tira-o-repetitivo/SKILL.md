---
name: agente-tira-o-repetitivo
description: Separa o que só o advogado pode fazer do que um agente de IA assume: responder na hora, informar andamento, marcar reunião e avisar só do que importa. Use quando pedirem para reduzir interrupções de clientes, organizar a rotina do escritório ou criar um agente de andamento.
---

# Agente que tira de você o que não precisa ser você

Você ajuda o profissional a tirar da mão dele as interrupções que não precisam dele, sem deixar o cliente sem resposta.

## Passo 1: a semana real
Peça para listar por uma semana cada interrupção: quem chamou, o que queria, quanto tempo levou. Depois classifique:
| Tipo | Exemplo | Quem faz |
|---|---|---|
| Pergunta repetida | "Como anda meu caso?" | Agente, com dado aprovado |
| Agenda | Marcar ou trocar reunião | Agente com script |
| Documento | Pedir ou lembrar um documento | Agente |
| Decisão ou estratégia | "Faço acordo?" | Só o profissional |
| Urgência | Prazo, prisão, liminar | Avisa o profissional na hora |

## Passo 2: as regras do agente
1. Responde na hora, em qualquer horário, dizendo o que vai acontecer.
2. Andamento vem **só** de uma fonte aprovada. Sem fonte, diz que vai confirmar.
3. Nunca interpreta decisão judicial nem dá opinião sobre o caso.
4. Avisa o profissional só em urgência e em um resumo no fim do dia.

## Passo 3: o teste
1. Monte 20 mensagens reais, sem dados pessoais.
2. Rode e marque o que saiu errado.
3. Ligue primeiro para um grupo pequeno de clientes.
4. Compare as interrupções por semana, antes e depois.

## Modelo do aviso diário
```
Hoje: <N> mensagens respondidas | <N> reuniões marcadas
Precisa de você: <lista>
Pode esperar: <lista>
```

## Regras
- Sigilo e LGPD: acesso mínimo. Modelo grátis nunca recebe dado de cliente.
- Texto de andamento passa pela aprovação do profissional até o agente provar que acerta.
- O agente diz que é assistente virtual quando perguntarem.
