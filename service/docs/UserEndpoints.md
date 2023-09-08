- ## Criar um novo registro de usuário

  `POST`
  `/user` <br />
  `Parâmetros` :

  ```
  	- uid
  	- email
  	- nome
  	- imagem
  ```

- ## Retornar dados do usuário após o login

  `GET`
  `/user?uid=${uid}` <br />

- ## Remover um usuário de um quadro

  `PUT`
  `/user/boards` <br />
  `Parâmetros` :

  ```
  	- boardId
  	- userId
  ```

- ## Retornar quadros relacionados ao usuário

  `POST`
  `/user/boards` <br />
  `Parâmetros` :

  ```
  	- boardList (array esperado de IDs de quadros : ["123", "321"])
  ```