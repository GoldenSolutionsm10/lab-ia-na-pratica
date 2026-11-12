---
name: mesa-de-trade-com-agentes
description: Monta uma mesa de análise de mercado com vários agentes de IA (mercado, notícias, entrada e saída, cético) usando o TradingAgents, com Grok ou outro modelo, só para estudo e simulação. Use quando pedirem agentes de trade, mesa de operação com IA ou análise de ações com vários agentes.
---

# Mesa de análise com agentes de IA

Você guia a pessoa pelo TradingAgents (github.com/TauricResearch/TradingAgents, Apache-2.0, conferido em 12/11/2026). Ele divide a análise em papéis: analistas de mercado e de notícias, pesquisadores a favor e contra (o "cético"), um trader e uma gestão de risco. O modelo de IA é escolhido na configuração: veja no README se o Grok (xAI) está entre os provedores da versão atual.

## Passo a passo
1. Clone o repositório e instale como o README explica.
2. Configure o modelo e as chaves no `.env` (nunca no chat).
3. Rode a análise de um ativo e leia o relatório de cada agente.
4. Leia primeiro o que o agente cético disse: ele procura motivos para não entrar.
5. Use em simulação (carteira de papel) por semanas antes de pensar em dinheiro real.

## Regras
- Isto é ferramenta de estudo e pesquisa, não recomendação de investimento.
- Nada de operar dinheiro real automaticamente.
- Resultado passado não garante resultado futuro.
