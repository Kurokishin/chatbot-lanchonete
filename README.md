<hr>

![Logo_CompassoUOL_Positivo](https://user-images.githubusercontent.com/94761781/212589731-3d9e9380-e9ea-4ea2-9f52-fc6595f8d3f0.png)
# 📑 Avaliação Sprint 7 - Programa de Bolsas Compass UOL / AWS e IFCE

Avaliação da sétima sprint do programa de bolsas Compass.uol para formação em machine learning para AWS.

<hr>
<p align="center">
  


## 📌 Tópicos 

- [🧾 Descrição do projeto](#-descrição-do-projeto)

- [⚙️ Ferramentas e Tecnologias](#-ferramentas-e-tecnologias)

- [📝 Requisitos e Execução](#%EF%B8%8F-código)

- [♾️ Equipe](#%EF%B8%8F-equipe)

- [📌 Considerações Finais](#-considerações-finais)

<hr>

## 🧾 Descrição do projeto 
Com base na [Documentação Amazon Lex](https://compasso-my.sharepoint.com/:f:/g/personal/lucas_sousa_compasso_com_br/Eph8d9BDeRhGhBzyoAYRLZUBhfjA54P1-5YHERGaN5_Osg?e=1ibFDI), foi realizada a construção de um chatbot utilizando o Amazon Lex V2 e o conecte a uma plataforma de mensageria.
A funcionalidade faz analogia ao atendimento online aos interessados nos salgados de uma fábrica de salgados(MegaLanches - nome fictício) 

<p align="justify">
<hr>

## ⚙️ Ferramentas e Tecnologias 

<a href="https://aws.amazon.com/pt/" target="_blank"> <img src="https://imgs.search.brave.com/GMxBwk4HNqhFJEmYkqXOW8kelyHphegTgfv8jGX3E3M/rs:fit:1200:1197:1/g:ce/aHR0cHM6Ly9naXN1/c2VyLmNvbS93cC1j/b250ZW50L3VwbG9h/ZHMvMjAxOC8wOC8y/MDAwcHgtQW1hem9u/X1dlYl9TZXJ2aWNl/c19Mb2dvLnN2Z18u/cG5n" alt="aws" width="40" height="40" title="AWS"/> </a><a href="https://docs.aws.amazon.com/pt_br/lexv2/latest/dg/what-is.html" target="_blank"> <img src="https://imgs.search.brave.com/bVZ4uQWr-3duPfutx8MysuJr104Mk89zeMApyYVzVjg/rs:fit:300:300:1/g:ce/aHR0cHM6Ly9zeW1i/b2xzLmdldHZlY3Rh/LmNvbS9zdGVuY2ls/XzcvM19hbWF6b24t/cmVrb2duaXRpb24u/NmFkOGEzYzFiOC5w/bmc" alt="firebase" width="40" height="40" title="AWS LexV2"/> </a> <a href="https://slack.com/intl/pt-br/media-kit" target="_blank"> <img src="https://imgs.search.brave.com/eEl2VJx5Re6JoRirC111bGSvKYC2Hj0Hltdn26O5pbA/rs:fit:1200:1200:1/g:ce/aHR0cHM6Ly9jZG4u/ZnJlZWJpZXN1cHBs/eS5jb20vbG9nb3Mv/bGFyZ2UvMngvc2xh/Y2stMS1sb2dvLXBu/Zy10cmFuc3BhcmVu/dC5wbmc" alt="firebase" width="40" height="40" title="AWS Lambda"/> </a>

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
![4](https://user-images.githubusercontent.com/94761781/221339201-189f750d-fad3-4dfe-a30a-3c7659d4fdfc.png)
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

*** observar integração ***
- Construção:   
  - Intents:    
    - lista de itents
  - Slots:    
    - Captação de informações presentes no texto;    
    - Solicitação de informações quando o slot não for reconhecido;    
    - Confirmação de informações;    
    - O chatbot deve captar ao menos 3 slots no decorrer do fluxo;
- O chatbot deve utilizar-se de menu com botões (Response Cards);
- Tratamento de erros (fallback);

## Integração com Slack

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

## Resultado da integração

![resultado](https://user-images.githubusercontent.com/103221427/221378685-fdcdf354-a830-4ed2-940f-7796337a2233.png)




















- Facebook
    - detalhar

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
  - Documentar detalhes sobre como a avaliação foi desenvolvida;
  - Dificuldades conhecidas;

<hr>


