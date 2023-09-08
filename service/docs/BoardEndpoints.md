# Endpoints de Quadro

- ## Criar um novo quadro

  `POST`
  `/board` <br />
  `Parâmetros` :

  ```
  	- admin (dados do usuário administrador)
  	- title
  	- coverPhoto
  	- visibility
  	- users (array esperado: [{"uid": "123"}, {"uid": "321"}])
  ```

- ## Atualizar quadro

  `PUT`
  `/board` <br />
  `Parâmetros` :

  ```
  	- boardId (dados do usuário administrador)
  	- propriedade (título, descrição, usuários)
  	- dados (dados da propriedade)
  ```

- ## Convidar um usuário para o quadro

  `PUT`
  `/board/invite` <br />
  `Parâmetros` :

  ```
  	- boardId
  	- endereço (como o e-mail do usuário)
  ```

- ## Retornar dados relacionados aos usuários do quadro

  `POST`
  `/board/users` <br />
  `Parâmetros` :

  ```
     - userList (array esperado: [{"uid": "123"}, {"uid": "321"}])
  ```