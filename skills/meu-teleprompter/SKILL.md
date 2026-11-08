---
name: meu-teleprompter
description: Monta um teleprompter próprio e gratuito que abre no celular, com o texto rolando por cima da câmera, a moldura do Reel e os botões que somem na hora de gravar. Use quando pedirem teleprompter, ler roteiro gravando, gravar olhando para a lente ou trocar os textos do teleprompter.
---

# Meu teleprompter

Você entrega um teleprompter em uma página só, sem aplicativo pago e sem conta. Os arquivos estão em `teleprompter/` nesta skill.

## Passo a passo
1. Peça os roteiros da pessoa, um por vídeo.
2. Copie a pasta `teleprompter/` para o projeto dela.
3. Reescreva `falas.js`: um item por vídeo, com `titulo`, `arquivo`, `dica` e `texto`. Linha em branco vira pausa.
4. Publique em um endereço com HTTPS, porque o navegador só libera a câmera assim. O caminho mais simples é a Vercel, no plano gratuito: `npx vercel deploy --prod` dentro da pasta.
5. Passe o link e diga para abrir no celular e permitir câmera e microfone.

## Regras
- Os textos ficam no `falas.js`, que vai junto com a página: quem tiver o link consegue ler. Não coloque dado de cliente nem senha.
- O vídeo fica no aparelho da pessoa. A página não envia a gravação para lugar nenhum.
- A gravação pelo navegador pode sair com qualidade menor que a do aplicativo Câmera. Se a pessoa notar, diga isso.
