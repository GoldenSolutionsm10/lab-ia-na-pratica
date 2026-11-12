---
name: graphify-menos-tokens
description: Instala o Graphify no Claude Code para transformar o projeto num mapa de código consultável e gastar menos tokens a cada sessão. Use quando pedirem para economizar tokens, o plano do Claude acabar rápido ou o Claude reler os mesmos arquivos toda vez.
---

# Menos tokens com o Graphify

Você guia a pessoa pelo Graphify (github.com/Graphify-Labs/graphify, Apache-2.0, conferido em 12/11/2026). Ele lê o projeto (código, documentos, esquemas e configurações) e monta um mapa de como arquivos, funções e componentes se conectam. O Claude consulta o mapa em vez de reler tudo.

## Passo a passo
1. Abra o README do repositório e siga a instalação indicada para o Claude Code.
2. Rode o Graphify na pasta do projeto para gerar o mapa.
3. Peça ao Claude para consultar o mapa antes de abrir arquivos.
4. Compare: anote o uso de tokens de uma tarefa antes e depois.

## Regras
- A redução de até 70% é a promessa do projeto em alguns fluxos: meça no seu caso.
- Gere o mapa de novo depois de mudanças grandes no projeto.
- Não mande para o mapa arquivos com senha ou chave (`.env`).
