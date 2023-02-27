<hr>

![Logo_CompassoUOL_Positivo](https://user-images.githubusercontent.com/94761781/212589731-3d9e9380-e9ea-4ea2-9f52-fc6595f8d3f0.png)
# 📑 Avaliação Sprint 7 - Programa de Bolsas Compass UOL / AWS e IFCE

Avaliação da sétima sprint do programa de bolsas Compass.uol para formação em machine learning para AWS.

<hr>
<p align="center">
  


## 📌 Tópicos 

- [🧾 Descrição do projeto](#-descrição-do-projeto)

- [⚙️ Ferramentas e Tecnologias](#%EF%B8%8F-ferramentas-e-tecnologias)

- [📝 Requisitos e Execução](#-requisitos-e-execuçãohands-on)

- [♾️ Equipe](#%EF%B8%8F-equipe)

- [📌 Considerações Finais](#-considerações-finais)

<hr>

## 🧾 Descrição do projeto 
Com base na [Documentação Amazon Lex](https://compasso-my.sharepoint.com/:f:/g/personal/lucas_sousa_compasso_com_br/Eph8d9BDeRhGhBzyoAYRLZUBhfjA54P1-5YHERGaN5_Osg?e=1ibFDI), foi realizada a construção de um chatbot utilizando o Amazon Lex V2 e o conecte a uma plataforma de mensageria.
A funcionalidade faz analogia ao atendimento online aos interessados nos salgados de uma fábrica de salgados(MegaLanches - nome fictício) 

<p align="justify">
<hr>

## ⚙️ Ferramentas e Tecnologias 

<a href="https://aws.amazon.com/pt/" target="_blank"> <img src="https://imgs.search.brave.com/GMxBwk4HNqhFJEmYkqXOW8kelyHphegTgfv8jGX3E3M/rs:fit:1200:1197:1/g:ce/aHR0cHM6Ly9naXN1/c2VyLmNvbS93cC1j/b250ZW50L3VwbG9h/ZHMvMjAxOC8wOC8y/MDAwcHgtQW1hem9u/X1dlYl9TZXJ2aWNl/c19Mb2dvLnN2Z18u/cG5n" alt="aws" width="40" height="40" title="AWS"/> </a><a href="https://docs.aws.amazon.com/pt_br/lexv2/latest/dg/what-is.html" target="_blank"> <img src="https://imgs.search.brave.com/bVZ4uQWr-3duPfutx8MysuJr104Mk89zeMApyYVzVjg/rs:fit:300:300:1/g:ce/aHR0cHM6Ly9zeW1i/b2xzLmdldHZlY3Rh/LmNvbS9zdGVuY2ls/XzcvM19hbWF6b24t/cmVrb2duaXRpb24u/NmFkOGEzYzFiOC5w/bmc" alt="firebase" width="40" height="40" title="AWS LexV2"/> </a> <a href="https://slack.com/intl/pt-br/media-kit" target="_blank"> <img src="https://imgs.search.brave.com/eEl2VJx5Re6JoRirC111bGSvKYC2Hj0Hltdn26O5pbA/rs:fit:1200:1200:1/g:ce/aHR0cHM6Ly9jZG4u/ZnJlZWJpZXN1cHBs/eS5jb20vbG9nb3Mv/bGFyZ2UvMngvc2xh/Y2stMS1sb2dvLXBu/Zy10cmFuc3BhcmVu/dC5wbmc" alt="firebase" width="40" height="40" title="Slack"/> </a><a href="https://developers.facebook.com/products/" target="_blank"> <img src="https://imgs.search.brave.com/Lm3QSaaOMnI19WcTOtDADCI5Z6ZaTeujhZrHElNP6co/rs:fit:650:240:1/g:ce/aHR0cDovL3d3dy5h/cnRpdC1rLmNvbS93/cC1jb250ZW50L3Vw/bG9hZHMvMjAxNC8w/OS9GYWNlYm9vay1E/ZXZlbG9wZXJzLUxv/Z28ucG5n" alt="firebase"  height="40" title="Slack"/> </a> 


<hr>

## 📝 Requisitos e Execução(Hands On)

#### Requisitos
- crie uma conta na [AWS](https://aws.amazon.com/pt/account/)
- acesse o serviço [LEX](https://slack.com/intl/pt-br/media-kit)

#### Execução
1 - Ao acessar o serviço na console, já uma breve aboradagem.... Clique em "Criar boot a partir de um modelo":
![01](https://user-images.githubusercontent.com/94761781/221339202-d0c91b13-a92a-4029-a767-4c9578d54738.png)

2 - De forma semelhante se já tiver alguns boots, haverá um outro rearranjo, mas configura a mesma situação anterior. Prossiga clicando em "Create Boot"
![1 5](https://user-images.githubusercontent.com/94761781/221339194-aef37fe9-98cb-496a-9244-e74396576e46.png)

3 - Na próxima visualização marque proceda com os componentes indicados e ao final clique em next
![2](https://user-images.githubusercontent.com/94761781/221339199-987f99b2-7cf6-4c0a-9aba-284c4431cfa1.png)
Na raia “IAM permissions”, selecione a opção “Create a role with basic Amazon Lex permissions”. Logo em seguida, selecione “não” na opção "Children 's Online Privacy Protection” e deixe tempo de sessão na escolha padrão (poderá ser alterado futuramente).

4 - A próxima tela se refere a configuração de todos os idiomas que o bot suportará. Selecione Português como opção, e deixar a Voice Interaction em 
``` "None". This is only a text based application” ```, 
![2 5](https://user-images.githubusercontent.com/94761781/221339196-e01f5c50-6256-4bf3-9025-d190c9cddb5e.png)

5 - Após a criação será solicitada a princípio a criação de Intents
![2 6](https://user-images.githubusercontent.com/94761781/221339198-b74b5efd-2906-4c3a-a9b4-b57294781ac9.png)

6 - Segue as respectivas itents utilizadas para o Chatboot
![3](https://user-images.githubusercontent.com/94761781/221339200-bfb74b51-9bae-494a-bcf9-f1aca4f62b26.png)

7 - Criadas Itens, pode-se prosseguir com a exploração da aba lateral
<img src="https://user-images.githubusercontent.com/94761781/221339201-189f750d-fad3-4dfe-a30a-3c7659d4fdfc.png" width="140">
``` Bot versions ```
 Possibilita o versionamento e controle de versões do bot.
```Idioma```
É a seção principal para o desenvolvedor. Nela, é possível criar intents e slots, que são a base do funcionamento de qualquer chatbot. 
```Deployment```
A opção de aliases serve para realizar o controle de versões e de ambientes de desenvolvimento.
Enquanto o versions possibilita a criação de versões, os aliases permitem a criação de ambientes
como homologação e produção, que apontam para versões desejadas no bot. Integrações com canais de comunicação podem ser realizadas nesta aba

8 - Sobre os Slots, observa-se os seguintes desenvolvidos para entrega desse chatbot
![5](https://user-images.githubusercontent.com/94761781/221339426-67b25a8b-ca9b-4e78-9399-f8027cf8add2.png)


#### Integração com Slack <a href="https://slack.com/intl/pt-br/media-kit" target="_blank"> <img src="https://imgs.search.brave.com/eEl2VJx5Re6JoRirC111bGSvKYC2Hj0Hltdn26O5pbA/rs:fit:1200:1200:1/g:ce/aHR0cHM6Ly9jZG4u/ZnJlZWJpZXN1cHBs/eS5jb20vbG9nb3Mv/bGFyZ2UvMngvc2xh/Y2stMS1sb2dvLXBu/Zy10cmFuc3BhcmVu/dC5wbmc" alt="firebase" width="15" height="15" title="Slack"/> </a>


O chatbot está sendo disponibilizado na seguinte plataforma:
  - Slack - [Conexão Slack](https://docs.aws.amazon.com/pt_br/lex/latest/dg/slack-bot-association.html);  

1 - Para realizar a integração, inicialmente criamos o bot conforme detalhado anteriormente 

2 - Realizamos um  [cadastro na plataforma Slack](https://slack.com/intl/pt-br/)

3 - Criamos a aplicação Slack na [Plataforma de Desenvolvedores](https://api.slack.com/)

![criando app](https://user-images.githubusercontent.com/103221427/221373306-2c9fbdfb-9053-4b95-ba18-2a7318a94ada.png)

4 - Definindo nome e configurações básicas para obtenção do token de verificação.

![criando nome](https://user-images.githubusercontent.com/103221427/221375218-98172466-fe99-412b-a740-f1181595e718.png)

![interatividade](https://user-images.githubusercontent.com/103221427/221375376-50dfb9a8-cae4-41eb-a0f4-f327c1bbcc5d.png)

5 - Em sequência, no menu esquerdo consultamos os tokens disponibilizados através dos campos:

> Settings > Basic Information

6 - Realizando configuração no console da AWS

![plataforma aws](https://user-images.githubusercontent.com/103221427/221376414-d09a9643-4540-4e0c-a513-2e1cd70fa6de.png)

Atribuindo nome à integração e selecionando o alias do bot criado e o idioma utilizado

![Config Integração](https://user-images.githubusercontent.com/103221427/221376543-25c118b4-3647-48b0-acbb-403268a34ebc.png)

7 - Em seguida, deve-se preencher os campos indicados no menu de **Configuração adicional** com os tokens obtidos no passo 5 e clicar em **Adicionar**

8 - Com o canal devidamente criado, selecione-o e anote o Endpoint e o Endpoint OAuth

9 - Voltando a página do slack, no menu **OAuth & Permissions**, foram realizadas as seguintes modificações: 

> **Redirect URLs** > Add New Redirect URL > Adicionar o Endpoint OAuth fornecido no passo 8

> **Scopes** > Add an OAuth Scope > Adicionar: chat:write e team:read

A página OAuth & Permissions deve ficar assim: 

![url slack](https://user-images.githubusercontent.com/103221427/221377760-73fe9f38-6fb0-43d9-8f19-75400e816ea6.png)

10 - Voltando ao menu **Interactivity e Shortcuts** devemos substituir a URL definida no passo 4 pelo Endpoint fornecido no console da AWS.

11 - No menu **Event Subscriptions** foram realizadas as seguintes modificações:

> **Enable Events** > Request URL > Adicionar o Endpoint fornecido no passo 8

> **Subscribe to bot events** > Add bot User event > Adicionar: message.im

A página Event Subscriptions deve ficar assim: 

![final config](https://user-images.githubusercontent.com/103221427/221378247-eaf9c37c-85da-4c13-a91b-68267ef652cd.png)

12 - Para finalizar no Menu **Manage Distribution em Settings** :
> Clique em **Add to Slack**

> Na solicitação de permissões selecione permitir

> Selecione o app e na aba Mensagens comece a interagir com o bot!

##### Resultado da integração

![resultado](https://user-images.githubusercontent.com/103221427/221378685-fdcdf354-a830-4ed2-940f-7796337a2233.png)


#### Integração com <a href="https://developers.facebook.com/products/" target="_blank"> <img src="https://imgs.search.brave.com/Lm3QSaaOMnI19WcTOtDADCI5Z6ZaTeujhZrHElNP6co/rs:fit:650:240:1/g:ce/aHR0cDovL3d3dy5h/cnRpdC1rLmNvbS93/cC1jb250ZW50L3Vw/bG9hZHMvMjAxNC8w/OS9GYWNlYm9vay1E/ZXZlbG9wZXJzLUxv/Z28ucG5n" alt="firebase" width="100" height="50" title="Slack"/> </a> 

Para integrar o bot criado no Amazon Lex V2 ao Facebook Messenger, você precisa seguir os seguintes passos:

1 - Crie um aplicativo no Facebook for Developers e adicione o Facebook Messenger como uma plataforma de produto.

- Acesse o site do Facebook for Developers em https://developers.facebook.com/ e faça login com sua conta do Facebook.
![01](https://user-images.githubusercontent.com/94761781/221447434-bafcc3c3-3b17-43fa-bf48-daa7876a93d5.png)

- Clique em "Meus Aplicativos" no canto superior direito da página e na sequência selecione "Criar Aplicativo".
![02](https://user-images.githubusercontent.com/94761781/221447439-ebbe9ba9-96c1-45a5-9222-96abbb1f4214.png)

- Selecione um tipo para sua Aplicação, clique em "Avançar" e digite um nome para o seu aplicativo. 

![03](https://user-images.githubusercontent.com/94761781/221447440-e288cb08-0efd-4c27-8756-08f564ed1a18.png)
![04](https://user-images.githubusercontent.com/94761781/221447442-c176def0-6cb2-4029-8da2-1e159c3bf98e.png)
    - não selecione a página agora, crie assim para ter mais disposição de serviços 

- Na página de inicial do aplicativo, seção de "Adicionar Produtos ao seu Aplicativo", localize e clique em "configurar" para adicionar a sua página e gerar o Token

    ![05](https://user-images.githubusercontent.com/94761781/221447444-27520eb5-6313-4721-8748-0cf6a658e9d3.png)

   Essa opção só irá aparecer se na criação do aplicativo você não selecioinar nem uma Página, pois assim terá mais privilégios sobre os serviços

- Na página de configuração do Messenger, selecione a página do Facebook que você deseja associar ao bot e clique em "Gerar Token de Acesso à Página".

![07](https://user-images.githubusercontent.com/94761781/221447453-4b9bc14a-3602-44ea-9c51-65dee49bd8ab.png)
![07 1](https://user-images.githubusercontent.com/94761781/221447450-2ead2a72-ec85-4b28-a22e-fc22feb21223.png)


    - Copie o token gerado e guarde-o em um local seguro.


2 - Configure o webhook do aplicativo do Facebook para apontar para o endpoint do Amazon Lex V2. Para fazer isso, você precisará fornecer a URL do endpoint do Amazon Lex V2 e um token de verificação.

- Na seção "Webhooks" da página de configuração do Messenger, clique em "Configurar Webhooks" e insira a URL do endpoint do Amazon Lex V2.
![08 00](https://user-images.githubusercontent.com/94761781/221447456-ddf7342b-3e80-4a9c-962b-a6eca0c9840e.png)
***ESSE TOKEN DE VERIFICAÇÃO É O ALIAS DA CRIAÇÃO DO ENDPOINT***

      - se ainda não houver endpoint vá na console em
      Lex > Bots  > Bot: MegaLanches > Channel integrations > Add channel  
      Selecione o Facebook e configure
   ![08 1](https://user-images.githubusercontent.com/94761781/221447459-604ddf77-9590-42ae-a9a7-f2245ed91d96.png)
   ![08 2](https://user-images.githubusercontent.com/94761781/221447460-66438245-10b8-4933-9b75-481be74f2b6e.png)
   ***App Secrret Key*** é chave secreta que está em configurações > básico
   ***Page Acess Token*** é o Token gerado na página


  ![08 4](https://user-images.githubusercontent.com/94761781/221447462-2028776a-d1da-4e1a-a92f-26bd9f2b8fbf.png)
- Selecione as opções de assinatura de eventos que você deseja receber e clique em "Verificar e Salvar".

3 - Teste o bot no Facebook Messenger.  
  -    <img src="https://user-images.githubusercontent.com/94761781/221450105-6c31b2c9-a41a-4bd6-b1e8-7cfedc87b506.jpeg" width="200">

Acesse a página: https://www.facebook.com/profile.php?id=100089482627701&mibextid=ZbWKwL



[Link detalhado da integração do Faceboook ao Lex](https://docs.aws.amazon.com/lex/latest/dg/fb-bot-association.html)

***
- (Opcional) Uso de conditional branching para controle de fluxos ([Doc Conditional Branching](https://docs.aws.amazon.com/pt_br/lexv2/latest/dg/paths-branching.html));

<hr>

## ♾️ Equipe
- Luan Ferreira
- Mylena Soares
- Jhonnatan Gonçalves
- Rafael Pereira

<hr>

## 📌 Considerações Finais
Desenvolver um chatbot Lex V2 integrado com Slack e Facebook Messenger nos apresentou alguns desafios. 
- Configuração: Configurar corretamente o bot no Amazon Lex, Slack e Facebook Messenger, dado que se deve seguir cuidadosamente as documentações e guias disponíveis para garantir que tudo esteja configurado corretamente.

- Teste e Ajuste: Testar e ajustar o bot para garantir que ele esteja funcionando corretamente pode levar tempo. É importante testar o bot em diferentes cenários para identificar problemas e ajustar suas respostas de acordo.

De modo geral, consideramos o projeto de chatbot Lex V2 integrado com Slack e Facebook Messenger incluindo os seguintes eixos de ênfase:

- Foco no usuário: É importante focar na experiência do usuário ao desenvolver o chatbot. Isso significa entender as necessidades dos usuários e projetar o bot para atender a essas necessidades de maneira eficaz...

- Monitoramento contínuo: É importante monitorar continuamente o chatbot para identificar problemas e oportunidades de melhoria. Isso pode envolver análise de dados e feedback dos usuários.

- Iteração constante: O desenvolvimento de chatbot é um processo contínuo e iterativo. É importante estar disposto a fazer ajustes e melhorias no bot com base em feedback e análise contínuos. considerações finais para um projeto de desenvolvimento de chatbot Lex V2 integrado com Slack e Facebook Messenger incluem:

O Programa de Bolsas é muito proveitoso e vem proporcionando cada vez mais novas experiências e skills, assim como evidenciado nesse documento, foi mais uma das excelentes abordagens avaliativas da equipe Compass Uol
<hr>


