# Como integrar VTEX com o Blip

![icone_github](https://github.com/Wilkor/doc-plugin-vtex/assets/34819624/70238f9f-7dd3-4639-8c0b-b2fcce923cbe)

Palavras-chave: VTEX, E-commerce, Disparos Ativos, Notificações de Pedido, Status VTEX.

## 1. Vídeo demonstrativo

Assista ao vídeo abaixo para conferir uma demonstração prática da extensão.

## 2. Introdução

O **VTEX** é uma extensão que permite integrar seu e-commerce VTEX com a plataforma Blip para realizar envios de notificações ativas baseadas no status dos pedidos.

## 3. Funcionalidades

O **VTEX** oferece as seguintes funcionalidades:
- Integração de e-commerce VTEX com o Blip para disparos ativos de mensagem.
- Mapeamento de status de pedidos VTEX (ex: invoiced, ready-for-handling, payment-approved, payment-pending) com templates específicos no Blip.
- Atualização e gestão dinâmica de templates por status VTEX.
- Pausa e inicialização do serviço a qualquer momento.

A extensão **VTEX** é suportada nos seguintes canais: WhatsApp / Blip Router.

## 4. Instalação e Configuração

Após ativar a extensão através da Blip Store, ela deve ser instalada no bot Router/Roteador. Após a ativação, você precisará seguir os passos de configuração abaixo:

- Ao lado de Home na tela principal, clique em Blip Store, depois no menu lateral, clique em extensões;
- Procure por **VTEX** e clique em ativar (Instalar em seu bot Router/Roteador);
- Após instalada a extensão, siga os passos abaixo:

### Configuração VTEX!

- Na tela de configuração, basta adicionar os headers `X-VTEX-API-AppToken`, `X-VTEX-API-AppKey` e URL (sua loja) que você consegue dentro da tela de ADM do seu E-commerce VTEX;
- Preencher conforme tela abaixo:

![image](https://github.com/Wilkor/doc-plugin-vtex/assets/34819624/83eeeaad-8e51-4beb-b302-7444284e6bbc)

### Configuração BLiP + VTEX

- Nesta tela, você irá informar algumas informações importantes para o funcionamento de seus disparos ativos;
- **Idioma**: Adicionar o idioma do seu template;
- **Chatbot**: Adicionar o chatbot em que você irá receber as notificações;
- **Bloco**: Aqui você vai adicionar o bloco específico onde o cliente vai cair quando ele responder à mensagem ativa;

**Status VTEX!**

- Nessa sessão, você vai vincular os status VTEX com os templates criados para cada um deles, por exemplo: status: `invoiced` -> template: `mensagem_invoiced_v1`.

Para mais informações sobre status, você pode consultar a página abaixo:
https://developers.vtex.com/vtex-rest-api/reference/listorders#order-status

![image](https://user-images.githubusercontent.com/34819624/194957037-edb5eee1-4ed7-48b5-a4e5-475d5e7b799a.png)

Feito o passo a passo acima, a tela será atualizada e mostrará a informação do serviço (onde está a seta vermelha indica os status do serviço), conforme tela abaixo:

![image](https://github.com/Wilkor/doc-plugin-vtex/assets/34819624/a0559e0f-a458-4a55-9ea2-8e1381113c2c)

Além de você poder pausar o serviço e inicializar a qualquer momento.

### Update de template BLIP versus status VTEX

Depois que habilitado o serviço, você poderá efetuar a atualização de um template, conforme tela abaixo:

![image](https://github.com/Wilkor/doc-plugin-vtex/assets/34819624/b553ad20-3f64-46c5-a611-323395dd67cd)

Na tela acima você tem a lista dos templates e status cadastrados com suas variáveis e na parte inferior da tela, você pode atualizar um status.

![image](https://github.com/Wilkor/doc-plugin-vtex/assets/34819624/f1b80b88-93ca-4c20-91d2-60f9bdb361c6)

Clicando em salvar, você atualiza o status com o template desejado.

## 5. Exemplos de Uso

Exemplos de mensagens por status:

- **invoiced** | Sendo variável `{{1}}` = data prevista para entrega e `{{2}}` para o URL de tracking do pedido:

![image](https://user-images.githubusercontent.com/34819624/195096355-b44da850-d071-494d-a468-fdd2591f1213.png)

- **ready-for-handling** e **handling** | Sendo variável `{{1}}` = Nome do cliente:

![image](https://user-images.githubusercontent.com/34819624/195097398-44a0fea3-9c0d-416f-9a41-62ae8a926ad8.png)

- **payment-approved** | Sendo variável `{{1}}` = Nome e `{{2}}` = data prevista para entrega:

![image](https://user-images.githubusercontent.com/34819624/195097774-9db773dd-09cb-4a00-b5a7-9146619da07e.png)

- **payment-pending** | Sendo variável `{{1}}` = Nome do cliente, `{{2}}` Código de barras e `{{3}}` link do boleto para pagamento:

![image](https://user-images.githubusercontent.com/34819624/195098138-ad234448-b264-4f0e-8c55-f0d961aa406e.png)

## 6. Suporte

Caso tenha alguma dúvida ou enfrente problemas com a extensão, entre em contato conosco pelos canais abaixo:

- **E-mail**: contato@wconsulting.tech
- **Telefone/WhatsApp**: 1191628-2384
