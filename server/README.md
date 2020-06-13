<h3 align="center">
    <img alt="Logo" title="#logo" width="300px" src="../assets/logo.svg">
</h3>

<p align="center">
  <a href="https://rocketseat.com.br">
    <img alt="Idea by Rocketseat" src="https://img.shields.io/badge/idea%20by-Rocketseat-%237519C1">
  </a>
  <a href="https://rocketseat.com.br">
    <img alt="Credits Rocketseat" src="https://img.shields.io/badge/credits%20-Rocketseat-%237519C1">
  </a>
   <a href="https://github.com/VictorGabrielMS">
    <img alt="Code by Victor Gabriel" src="https://img.shields.io/badge/code%20by-Victor Gabriel-%23E02041">
  </a>
</p>


<p align="center">
  <a href="https://developer.mozilla.org/pt-BR/docs/Web/JavaScript">
    <img alt="Javacript" src="https://img.shields.io/badge/Javacript-%23D1CB36">
  </a>
  <a href="https://nodejs.org/en/">
    <img alt="Node.js" src="https://img.shields.io/badge/Node.js-%2341B879">
  </a>
</p>


## <img alt="bethehero" src="../assets/icon.png" height="15"> Be The Hero

- [Sobre](#sobre)
- [Tecnologias utilizadas](#tecnologias-utilizadas)
- [Rotas](#rotas)
- [Faça um clone e use](#como-usar)
- [Como contribuir](#como-contribuir)

<a id="sobre"></a>

## :interrobang: «» Sobre

O backend da aplicação <strong>Be the hero</strong>

O lado com todas as regras de negócio da palicação, uma _API Rest_, onde as requisições são processadas e uma resposta em formato JSON e devolvida. 


## :diamonds: «» Tecnologias utilizadas
<a id="tecnologias-utilizadas"></a>

O projeto foi desenvolvido utilizando as seguintes tecnologias:

- [Node.js](https://nodejs.org/en/)
- [Sqlite](https://www.sqlite.org/index.html)


<a id="rotas"></a>

## :space_invader: «» Rotas

> #### $GET ᚛ http://aplication_url/ongs
> - rota usada para listar todas as ongs cadastradas na aplicação
>
> <br>
>
> #### $POST ᚛ http://aplication_url/ongs
> - rota usada para cadastrar uma nova ong
> - **PARÂMETROS » Enviados pelo corpo da requisição**:
>   - name → _nome da ong que será cadastrada_ 
>   - email → _email da ong que será cadastrada_
>   - whatsapp → _numero de contato da ong que será cadastrada_
>   - city → _cidade da ong que será cadastrada_
>   - uf → _estado da ong que será cadastrada_
>
> <br>
>
> #### $GET ᚛ http://aplication_url/profile
> - rota usada para listar os casos de um ong específica
> - **PARÂMETROS » Enviado pelo cabeçalho "_authorization_"**:
>   - ong_id → _identificador de uma ong que já esta cadastrada_

<br>

> #### $POST ᚛ http://aplication_url/sessions
> - rota usada para criar a sessão de uma ong que já foi cadastrada na aplicação
> - **PARÂMETROS » Enviados pelo corpo da requisição**:
>    - id → _identificador de uma ong que já esta cadastrada_

<br>

> #### $GET ᚛ http://aplication_url/incidents
> - rota usada para listar todos os casos cadastrados na aplicação
> - **PARÂMETROS » Enviados via parâmetros _query_** :
>   - page → _numero da pagina que deve ser exibida, por padrão é igual a 1_
>
> <br>
>
> #### $POST ᚛ http://aplication_url/incidents
> - rota usada para cadastrar um novo caso
> - **PARÂMETROS »**
>   - **Enviados pelo corpo da requisição**:
>     - title → _titulo do caso que será cadastrado_
>     - description → _descrição do caso que será cadastrado_
>     - value → _preço do caso que será cadastrado_
>   - **Enviados pelo cabeçalho "_authorization_"**:
>     - ong_id → _identificador da ong que está cadastrando o caso_
>
> <br>
>
> #### $DELETE ᚛ http://aplication_url/incidents/:id
> - rota usada para deletar um caso que já foi cadastrado
> - **PARÂMETROS »** 
>   - **Enviados pela url requisição**:
>      - id → _identificador do caso_
>   - **Enviados pelo cabeçalho "_authorization_"**:
>      - ong_id → _identificador da ong que está cadastrando o caso_

<a id="como-usar"></a>

## :octocat: «» Clone este repositório

1. Faça um clone :

```sh
  $ git clone https://github.com/victorgabrielms/bethehero.git
```

2. Executando as aplicações:

```sh
  $ cd server
  $ npm install
  $ npm run start
```

<a id="como-contribuir"></a>

## :dart: «» Como contribuir

- Faça um _Fork_ deste repositório;
- Crie uma _branch_ com a sua feature: `git checkout -b my-feature`
- _Commit_ suas mudanças: `git commit -m 'feat: My new feature'`
- Faça um _push_ da sua branch: `git push origin my-feature`


