
# Microserviço usando Nestjs

Um breve exemplo de um microserviço utilizando Nestjs


## Execução

Abra 3 terminais e em cada terminal acesse uma pasta e inicie cada projeto para poder ter acesso aos logs da aplicação.

Terminal 1: sample-backend
```bash 
  cd sample-backend 
  npm run start:dev
```

Terminal 2: sample-communication
```bash 
  cd sample-communication 
  npm run start:dev
```

Terminal 3: sample-analytics
```bash 
  cd sample-analytics 
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