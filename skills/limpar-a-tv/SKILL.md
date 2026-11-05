---
name: limpar-a-tv
description: Usa o projeto Clean Your TV com o Claude Code para tirar anúncios e aplicativos de fábrica de uma Android TV ou Google TV e instalar uma tela inicial nova, com backup. Use quando pedirem para limpar a TV, tirar propaganda da TV ou trocar a tela inicial.
---

# Limpar a TV com o Claude Code

Você guia a pessoa pelo projeto Clean Your TV (github.com/Gathin23/cleanyourtv, conferido em 05/11/2026). Use os scripts do repositório: é neles que ficam o backup e o registro para restaurar.

## Pré-requisitos
- Android TV ou Google TV na mesma rede Wi-Fi do computador.
- Python 3, JDK de 17 a 22 e Android SDK 34 com build-tools 34.
- Para LG (webOS), Samsung e outros modelos, confira o README: há versões da comunidade, como github.com/lasharor/cleanyourtv-WebOS. São outros projetos: leia antes.

## Passo a passo
1. **Na TV:** Configurações → Preferências do dispositivo → Sobre → aperte OK em **Build** sete vezes. Volte, abra Opções do desenvolvedor e ligue **Depuração USB**.
2. **No computador:** `git clone https://github.com/Gathin23/cleanyourtv` e abra a pasta no Claude Code.
3. Cole o conteúdo de `PROMPT.md` e informe o modelo da TV.
4. Aceite "Permitir depuração USB?" na TV.
5. Responda o checklist: apps que usa, ordem do menu, se mantém assistente de voz, Chromecast e atualizações.
6. Confira cada etapa com as capturas de tela tiradas da TV.

## Regras
- Confirme o modelo antes de mexer. Confira se a TV aparece nas listas do repositório.
- Faça o backup antes de qualquer desligamento e mostre onde ele ficou.
- Explique que a pessoa assume o risco: pode afetar a garantia ou recursos da TV.
- Mexa só na TV da própria pessoa.
- A licença do projeto não é uma licença comum: leia o arquivo LICENSE antes de usar para outra pessoa ou vender.
- Terminou? Desligue a depuração se a pessoa não for mais usá-la.
