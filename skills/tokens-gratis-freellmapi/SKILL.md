---
name: tokens-gratis-freellmapi
description: Instala o FreeLLMAPI, que junta provedores gratuitos de modelos de IA em um único endereço e troca sozinho quando um atinge o limite. Use quando pedirem tokens grátis, API gratuita de IA ou como gastar menos com modelos.
---

# Tokens grátis com o FreeLLMAPI

Você instala o FreeLLMAPI (github.com/tashfeenahmed/freellmapi, MIT, conferido em 05/11/2026) e liga a ferramenta da pessoa nele.

## O que é
Um servidor que roda na máquina da pessoa. Ela cadastra as chaves gratuitas de cada provedor e usa um endereço único. Estourou o limite de um, ele passa para o próximo.

## Passo a passo
1. Confira se o Docker está instalado.
2. Leia o script com a pessoa antes de rodar: https://freellmapi.co/install.sh
3. Instale: `curl -fsSL https://freellmapi.co/install.sh | bash`
4. Abra http://localhost:3001
5. Na página **Keys**, a pessoa cola as chaves dos provedores que quiser, ela mesma. Comece por 2 ou 3.
6. Ordene a **Fallback Chain**: o melhor modelo primeiro.
7. Pegue a chave unificada na mesma página e aponte a ferramenta para o endereço local. Confira no README o caminho atual da API.
8. Faça um teste e veja qual modelo respondeu.

## Regras
- A cota real depende de cada provedor e muda sem aviso. Confira na tela, não prometa número.
- **Dado de cliente nunca passa por aqui.** Provedor gratuito pode usar o que recebe. Use só com dado público.
- Respeite os termos de cada provedor.
- Chave nunca no chat: a pessoa cola na página ou no `.env`.
- Não exponha a porta na internet sem proteção.
- Para trabalho que não pode falhar, tenha um modelo pago de reserva.
