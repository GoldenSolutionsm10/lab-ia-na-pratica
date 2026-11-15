---
name: bloquear-propaganda-da-casa
description: Instala o Pi-hole num computador velho ou Raspberry Pi com Linux para bloquear anúncios em todos os aparelhos do Wi-Fi de casa, com painel do que foi barrado. Use quando pedirem para tirar propaganda da casa inteira.
---

# Bloquear propaganda em todo aparelho da casa

Você guia a pessoa pelo projeto Pi-hole (github.com/pi-hole/pi-hole, 62 mil estrelas, conferido em 15/11/2026). Siga o README e a documentação oficial do projeto; se algo aqui divergir, vale o README.

## O que ele faz
Filtra a internet da casa: o pedido de propaganda é barrado antes de chegar ao celular, à TV ou ao jogo. Mostra um painel com o que foi bloqueado.

## Onde roda
Linux num computador velho ou Raspberry Pi (pi-hole.net). Não tira o anúncio do YouTube, que vem junto com o vídeo.

## Passo a passo
1. Instale Linux no computador velho (o README lista os sistemas suportados).
2. Rode o instalador oficial indicado no README.
3. Anote o endereço e a senha do painel no fim da instalação.
4. No roteador, troque o DNS para o endereço do Pi-hole.
5. Abra o painel e veja os bloqueios do dia.

## Regras
- Mexer no roteador derruba a internet se der errado: anote a configuração antiga antes.
- Algum site pode quebrar: libere no painel.
- Antes de instalar, leia o README do repositório com a pessoa e confirme o sistema dela.
- Licença: veja o LICENSE do repositório. Leia o arquivo LICENSE antes de usar para outra pessoa ou vender.
