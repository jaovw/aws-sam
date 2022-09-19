# aws-sam
AWS CLI and SAM CLI

 ## Desc
 
 Criando um projeto Serverless com AWS CLI e SAM CLI. Realizando eventos em uma Lambda function.
 
 Sendo o SAM - Serverless Aplication Module, funciona de maneira semelhante ao serverless. 
 
 Com vantagens de 
  - testes e deploys locais 
  - push para o AWS Cloud.
  - fornece uma API Geteway
 
 
 Projeto desenvolvido e testado com Docker :whale2:

## __GETTING STARTED__

Criando o projeto:
```
$ sam init
```
Realizando o build, dentro do diretorio do projeto:
```
$ sam build
```
Chamando o handler:
```
$ sam local invoke
```
:warning: Necessario ter o container com status running :warning:

### :rocket: __DEPLOY__

Para deploy guiado com opcoes:
```
$ sam deploy --guided
```

Realizando o deploy local:
```
$ sam local start-api
```
:exclamation: Ira rodar a API no http://127.0.0.1:3000/hello | sempre com a rota do get

:warning: Para alteracos necessario refazer o build :warning:

## :bulb:__TIPS__

Rodando funcoes diretamente:

```
$ sam local invoke "_name_" -e events/event.json
```
Utilizar o .yml para checar o nome da sua funcao
