---
name: comentario-direct-chatbotx
description: Instala o ChatbotX em VPS própria e monta a automação comentou a palavra, recebeu resposta pública e direct no Instagram, com as armadilhas da Meta já resolvidas. Use quando pedirem comentário para direct, alternativa grátis ao ManyChat ou automação por palavra-chave.
---

# Seu próprio ManyChat com o ChatbotX

Antes de começar, peça: domínio do painel, conta profissional do Instagram, Página do Facebook ligada a ela e o IP de quem vai usar o painel. Segredo nunca passa pelo chat.

Repositório: github.com/ChatbotXIO/ChatbotX. Não use a pasta `enterprise`, que tem licença comercial.

## Passos
1. Faça snapshot da VPS. Suba o ChatbotX por Docker Compose (`chatbotx-docker-compose`), atrás de HTTPS.
2. Deixe o painel restrito por IP. Libere ao público só as rotas de webhook e arquivos públicos.
3. Crie um app da Meta do tipo empresa, no portfólio que será verificado. Adicione os casos de uso de Instagram e Messenger.
4. Conecte pela rota "Instagram via Facebook" e confira as permissões antes. Permissão faltando dá "Invalid Scopes".
5. Coloque a política de privacidade em URL pública, com dados, finalidades e exclusão, e salve no app.
6. Verifique o webhook e assine os campos `comments` e `messages`.
7. Crie a regra. Quem clica em Criar é o dono da conta.
8. **Publique o app.** Sem publicar, a Meta não entrega os comentários, mesmo com testador aceito.
9. Teste com conta testadora e depois com duas contas sem função no app.

## Armadilhas
- Comentário feito antes de publicar o app não é reenviado.
- "Uma resposta por pessoa por publicação" faz a mesma conta não disparar de novo.
- O modo "Contém" ignora maiúscula e acento e procura o trecho dentro do comentário. Não existe "parecido": cadastre a raiz e as variações.
- Palavra curta dispara sem querer no modo "Contém" ("dev" está em "deve"). Use uma regra separada com "Coincidência exata" para as curtas.
- Sem acesso avançado, o log mostra erro #200 ao ler o perfil e o contato fica sem nome. Não use o nome da pessoa no texto.
- Avise no comentário público para conferir Pedidos de mensagem: quem não segue o perfil pode receber lá.
- No Business Suite, entre pelo Facebook. Pelo Instagram, as configurações podem ficar bloqueadas.
- Virar Provedor de Tecnologia é apresentado pela Meta como irreversível. Teste antes de aceitar.
- A documentação da Meta pede análise aprovada para webhooks de comentários. Se funcionar sem ela, trate como instável e não prometa ao cliente.

## Antes de entregar
Grave o fluxo, corte contatos e dados de terceiros e mostre o resultado ao dono da conta. Nada vai ao público sem o "sim" dele.
