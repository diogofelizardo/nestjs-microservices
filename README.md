
# Microserviço usando Nestjs

Um breve exemplo de um microserviço utilizando Nestjs

A aplicação Backend se encarrega de cadastrar o usuário em tempo de execução e em seguida enviar uma mensagem para os 2 microserviços communication e analytics, o communication pode ser utilizado para enviar um email dando boas vindas ao usuario cadastrado e o analytics pode ser usado como uma especie de analise para verificar a data e hora que o usuário foi cadastrado, é um simples exemplo da utilização de microserviços.

## Rodando localmente

Clone o projeto

```bash
  git clone https://github.com/diogofelizardo/nestjs-microservices.git
```

Entre no diretório do projeto

```bash
  cd nestjs-microservices
```

Abra 3 terminais e em cada terminal acesse uma pasta e instale as dependencias e inicie cada projeto para poder ter acesso aos logs da aplicação.

Terminal 1: sample-backend
```bash 
  cd sample-backend 
  npm install
  npm run start:dev
```

Terminal 2: sample-communication
```bash 
  cd sample-communication 
  npm install
  npm run start:dev
```

Terminal 3: sample-analytics
```bash 
  cd sample-analytics 
  npm install
  npm run start:dev
```


## Documentação da API

#### Cadastrando um Usuário

```http
  POST localhost:3000/
```

| Parâmetro  | Tipo     | Descrição                           |
| :--------- | :------- | :---------------------------------- |
| `email`    | `string` | **Obrigatório**. Informe um email.  |
| `password` | `string` | **Obrigatório**. Informe uma senha. |

![Exemplo POST](/assets/insomnia_post.png)

#### Retorna todos os Usuários cadastrados

```http
  GET localhost:3000/analytics
```
![Exemplo GET](/assets/insomnia_get.png)



## Logs da Aplicação

#### Terminal Log Communications App
![Exemplo GET](/assets/terminal_log_communications.png)

#### Terminal Log Analytics App
![Exemplo GET](/assets/terminal_log_analytics.png)


## Referência

 - [Nest.js Microservices Tutorial in 20 Minutes](https://www.youtube.com/watch?v=C250DCwS81Q)



## Feedback

Se você tiver algum feedback, por favor nos deixe saber por meio de felizardo.diogo@gmail.com

