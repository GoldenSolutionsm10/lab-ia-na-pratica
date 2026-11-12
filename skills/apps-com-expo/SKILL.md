---
name: apps-com-expo
description: Usa as skills oficiais da Expo (github.com/expo/skills) com o Claude Code para criar um aplicativo completo para iPhone e Android, testar no simulador, atualizar e publicar nas lojas. Use quando pedirem para criar um app, transformar um site em aplicativo ou publicar na App Store e no Google Play.
---

# Apps com as skills da Expo

Você guia a pessoa pelo repositório oficial github.com/expo/skills (licença MIT, conferido em 12/11/2026). Ele traz skills para telas, animações, design, atualizações e publicação. O Claude escolhe a skill certa pelo pedido.

## Pré-requisitos
- Node.js LTS e o Claude Code.
- Celular com o app Expo Go, ou simulador (Xcode no Mac para iPhone, Android Studio para Android).
- Para publicar: conta de desenvolvedor da Apple e do Google Play, e conta grátis na Expo.

## Passo a passo
1. Instale as skills seguindo o README do repositório expo/skills.
2. Peça o app em português: para quem é, as telas e o que cada botão faz.
3. Rode `npx expo start` e abra no Expo Go ou no simulador.
4. Ajuste tela por tela: um pedido por vez.
5. Para publicar, siga a skill de build e envio (EAS) do repositório.

## Regras
- Descreva o app antes de escrever código e confirme com a pessoa.
- Chaves das lojas e senhas nunca vão no chat: ficam no painel da Expo ou em `.env`.
- Teste no aparelho antes de publicar.
- Publicar nas lojas pede contas pagas da Apple e do Google: avise antes.
