![N|Solid](https://raw.githubusercontent.com/Wilkor/img-clonebots/main/logoParseHorizontal.jpeg)


# Como utilizar a extensão VTEX!

Muito simples, basta seguir o passo a passo abaixo para ativar e configurar sua extensão:

 - Ao lado de Home na tela principal, clique em Blip Store, depois no menu lateral, clique em extensões;
 - Procure por **VTEX** e clique em ativar (Instalar em seu bot Router/Roteador);
 - Após instalado a extensão, siga os passos abaixo;
 
 # Configuração VTEX!
 
  - Na tela de configuração,  basta adicionar os headers X-VTEX-API-AppToken, X-VTEX-API-AppKey e URL(sua loja) que você consegue dentro da tela de ADM do seu E-commerce VTEX
  - Preencher conforme tela abaixo 
 
![image](https://github.com/Wilkor/doc-plugin-vtex/assets/34819624/83eeeaad-8e51-4beb-b302-7444284e6bbc)
  
   # Configuração BLiP + VTEX
  - Nesta tela, você irá informar algumas informações importantes para o funcionamento de seus disparos ativos;
  - Idioma: Adicionar o idioma do seu template;
  - Chabot: Adicionar o chatbot que você irá receber as notificações
  - Blco: Aqui você vai adicionar o bloco especifico onde o cliente vai cair quando ele reponder a mensagem ativa;
  
   **Status VTEX!**
  
  - Nessa sessão, você vai vincular os status VTEX com os templates criados para cada um deles, por exemplo: status: invoiced -> tempalte: mensagem_invoiced_v1
  
  Para mais informações sobre status, você pode consultar a pagina abaixo:
  
  https://developers.vtex.com/vtex-rest-api/reference/listorders#order-status

![image](https://user-images.githubusercontent.com/34819624/194957037-edb5eee1-4ed7-48b5-a4e5-475d5e7b799a.png)




 Feito o passo a passo acima, a tela será atualizada e mostrará a informação do serviço (onde esta a seta vermelha indica os status do serviço), conforme tela abaixo:
 
![image](https://github.com/Wilkor/doc-plugin-vtex/assets/34819624/a0559e0f-a458-4a55-9ea2-8e1381113c2c)

 Além de você poder pausar o serviço e inicializar a qualquer momento.
 
 
# Update de template BLIP  versus status VTEX
 
 Depois que habilitado o serviço, você poderá efetuar a atualização de um template, conforme tela abaixo:
 
 ![image](https://github.com/Wilkor/doc-plugin-vtex/assets/34819624/b553ad20-3f64-46c5-a611-323395dd67cd)
 
  Na tela acima você tem a lista dos templates e status cadatrado com suas variaveis e na parte inferior da tela, você pode atualizar um status.
  
![image](https://github.com/Wilkor/doc-plugin-vtex/assets/34819624/f1b80b88-93ca-4c20-91d2-60f9bdb361c6)

Clicando em salvar, você atualiza o status com o template desejado.

# Exemplos de mensagens por status

 - invoiced | Sendo variavel {{1}} = data prevista para entrega e {{2}} para o url de tracking do pedido
  
 ![image](https://user-images.githubusercontent.com/34819624/195096355-b44da850-d071-494d-a468-fdd2591f1213.png)

- ready-for-handling e handling | Sendo variavel {{1}} = Nome do cliente

![image](https://user-images.githubusercontent.com/34819624/195097398-44a0fea3-9c0d-416f-9a41-62ae8a926ad8.png)

- payment-approved | Sendo variavel {{1}} = Nome e {{2}} = data prevista para entrega

![image](https://user-images.githubusercontent.com/34819624/195097774-9db773dd-09cb-4a00-b5a7-9146619da07e.png)

- payment-pending | Sendo variavel {{1}} = Nome do cliente, {{2}} Código de barras e {{3}} link do boleto para pagamento

![image](https://user-images.githubusercontent.com/34819624/195098138-ad234448-b264-4f0e-8c55-f0d961aa406e.png)

 Em caso de duvidas, você pode entrar em contato conoscos para tirar qualquer tipo de duvida sobre a configuração da extensão
 
 Email: contato@pontoparse.net

