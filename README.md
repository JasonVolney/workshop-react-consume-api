---
description: >-
  Neste tutorial vamos ajudá-lo a criar um aplicativo Web utilizando React para
  consumir uma API
---

# workshop-react-consuming-api

## O que é React?

O React é uma biblioteca JavaScript de código aberto com foco em criar interfaces de usuário em páginas web. É mantido pelo Facebook, Instagram, outras empresas e uma comunidade de desenvolvedores individuais. É utilizado nos sites da Netflix, Imgur, Feedly, Airbnb, SeatGeek, HelloSign, Walmart e outros. Se preferir [clique aqui](https://www.youtube.com/watch?v=cEczlv669Oo) para assistir a um video e ter mais informações sobre React. 

![](.gitbook/assets/luke-chesser-lg8toawe8wq-unsplash.jpg)

Aqui está o link do repositório do projeto: [https://github.com/facebook/react](https://github.com/facebook/react).

## Preparação do ambiente

A primeira coisa que precisamos fazer antes de iniciar nosso projeto é garantir que temos o [NodeJs](https://nodejs.org/en/download/) instalado em nosso sistema**.** Para isto, abra um terminal **Ctrl + R** e digite `cmd` agora no seu prompt de comando digite `node -v` assim saberemos qual a versão do node instalada. Caso, retorne um erro significará que o NodeJs não está instalado, então [clique aqui](https://nodejs.org/en/download/) e baixe o NodeJs versão LTS, conforme seu sistema operacional e instale na sua máquina. Para instalar o Node é só dar next, next e finish. =\) 😉 Após a instalação concluída, repita a operação para verificar a versão.

![](.gitbook/assets/node%20%281%29.png)

Pronto! O NodeJs foi instalado com sucesso! 🥳 🎉 

![](.gitbook/assets/node.png)

O próximo passo é instalar a IDE para fazer o código do nosso projeto, caso não tenha instalado em sua máquina [clique aqui](https://code.visualstudio.com/download) para baixar o VSCode. 

![Lembrando que todas as ferramentas que vamos utilizar s&#xE3;o Open Sources.](.gitbook/assets/vscode.png)

 Uma vez instalado o VSCode, vamos criar o nosso projeto. 

O NodeJs tem seu próprio gerenciador de dependências, ele nos permite instalar outros pacotes que iremos precisar no nosso projeto. O Yarn também é um gerenciador de dependências.

Primeiro, abra um prompt de comando, digite ou copie o comando abaixo:

```text
npm install -g yarn
```

Agora você pode conferir a versão do yarn digitando `yarn -v`

![](.gitbook/assets/yarn.png)

Vamos usar o comando a seguir para instalar o gerador de aplicativos do React. Se quiser saber mais sobre o `create-react-app` pode conferir a documentação [aqui](https://create-react-app.dev/).

`yarn global add create-react-app`



[JSON](https://www.json.org/json-en.html) 

[https://jsonplaceholder.typicode.com/](https://jsonplaceholder.typicode.com/)





{% api-method method="get" host="" path="" %}
{% api-method-summary %}

{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="" type="string" required=false %}

{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="" path="" %}
{% api-method-summary %}

{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="" type="string" required=false %}

{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="" path="" %}
{% api-method-summary %}

{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="" type="string" required=false %}

{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.cakes.com" path="/v1/cakes/:id" %}
{% api-method-summary %}
Get Cakes
{% endapi-method-summary %}

{% api-method-description %}
This endpoint allows you to get free cakes.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="id" type="string" %}
ID of the cake to get, for free of course.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% api-method-parameter name="Authentication" type="string" required=true %}
Authentication token to track down who is emptying our stocks.
{% endapi-method-parameter %}
{% endapi-method-headers %}

{% api-method-query-parameters %}
{% api-method-parameter name="recipe" type="string" %}
The API will do its best to find a cake matching the provided recipe.
{% endapi-method-parameter %}

{% api-method-parameter name="gluten" type="boolean" %}
Whether the cake should be gluten-free or not.
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Cake successfully retrieved.
{% endapi-method-response-example-description %}

```
{    "name": "Cake's name",    "recipe": "Cake's recipe name",    "cake": "Binary cake"}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Could not find a cake matching this query.
{% endapi-method-response-example-description %}

```
{    "message": "Ain't no cake like that."}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



