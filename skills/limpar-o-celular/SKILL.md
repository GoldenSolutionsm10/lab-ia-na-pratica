---
name: limpar-o-celular
description: Usa o Universal Android Debloater Next Generation (UAD-ng) com o Claude Code para desligar aplicativos de fábrica e propaganda de um celular Android, sem root e com volta garantida. Use quando pedirem para limpar o celular, tirar bloatware, economizar bateria ou desligar apps que vêm de fábrica.
---

# Limpar o celular com o Claude Code

Você guia a pessoa pelo UAD-ng (github.com/Universal-Debloater-Alliance/universal-android-debloater-next-generation, conferido em 12/11/2026). Ele já traz a lista do que é seguro desligar em cada marca (Samsung, Xiaomi, Motorola e outras).

## Pré-requisitos
- Celular Android com cabo USB ou na mesma rede Wi-Fi (depuração sem fio, Android 11 ou mais novo).
- Computador com Windows, macOS ou Linux e o ADB (Android Platform Tools) instalado.
- Sem root.

## Passo a passo
1. **No celular:** Configurações → Sobre o telefone → toque sete vezes em **Número da versão**. Abra Opções do desenvolvedor e ligue **Depuração USB** (ou Depuração por Wi-Fi).
2. **No computador:** instale o ADB e baixe o UAD-ng pela página de Releases do repositório.
3. Conecte o celular e aceite "Permitir depuração?" na tela.
4. Abra o UAD-ng: ele lista os pacotes do aparelho com a marca de risco de cada um.
5. Comece só pelos marcados como **Recomendado**. Desligue poucos de cada vez e use o celular um dia antes do próximo lote.
6. Para voltar atrás: na mesma tela, reative o pacote. Nada é apagado de vez.

## Regras
- Mostre o nível de risco antes de desligar qualquer pacote. Pacotes **Expert** e **Unsafe** só com a pessoa ciente.
- Nunca desligue pacotes do sistema que a pessoa não reconhece sem ler a descrição do próprio UAD-ng.
- Exporte a lista do que foi desligado (o UAD-ng salva) e diga onde ficou.
- Mexa só no celular da própria pessoa.
- Licença do projeto: GPL-3.0. Leia antes de redistribuir.
- Terminou? Desligue a depuração.
