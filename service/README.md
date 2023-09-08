# Índice

- [Configuração](#Configuração)
- [Variáveis de Ambiente](#Variáveis-de-Ambiente)
- [Documentação](#Documentação)


# Configuração
 - Crie um arquivo firebaseConfig.json no diretório raiz (raiz do serviço).
 - Gere uma nova chave para o Firebase admin-sdk [aqui](https://console.firebase.google.com/project/_/settings/serviceaccounts/adminsdk).
 - Copie o conteúdo para dentro do arquivo firebaseConfig.json.
 - Deve ficar parecido com isto:

 ```json
 {
  "type": "service_account",
  "project_id": "",
  "private_key_id": "",
  "private_key": "",
  "client_email": "",
  "client_id": "",
  "auth_uri": "",
  "token_uri": "",
  "auth_provider_x509_cert_url": "",
  "client_x509_cert_url": ""
}
 ```

```bash
# Instale as dependências
$ npm install

# Para implantar
$ serverless deploy

# Para testar em seu ambiente local
$ serverless offline
```

# Variáveis de Ambiente

Usando o Firebase Realtime DB.

``` 
DATABASE_URL=XXX
SLS_DEBUG=*
```

# Documentação

### Pontos Finais

|[USUÁRIO](./docs/UserEndpoints.md) | [QUADRO](./docs/BoardEndpoints.md) | [LISTA](./docs/ListEndpoints.md) | [TAREFA](./docs/TaskEndpoints.md)
|:-------------                    | :-------------                   | :----------                    |  :----------                
| `POST /user`                     | `PUT, POST /board`               | `PUT, POST /list`              |  `POST /task`               
| `GET /user`                      | `PUT /board/invite`              | `PUT /list/rename`             |  `PUT /task-reorder`
| `PUT, POST /user/boards`         | `POST /board/users`              | `PUT /list/remove`             |  `PUT /task-switch`
|                                  |                                  |                                |  `PUT /task-update`