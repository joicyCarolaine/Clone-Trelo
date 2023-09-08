- ## Criar uma nova lista

  `POST`
  `/list` <br />
  `Parâmetros` :

  ```
  	- boardId
  	- lista (342(id da lista) : {id, taskIds:[], title})
  	- listOrder (array de IDs de listas : ["123", "321", "342"])
  ```

- ## Reordenar listas

  `PUT`
  `/list` <br />
  `Parâmetros` :

  ```
  	- boardId
  	- listOrder (array de IDs de listas : ["342", "321", "123"]) 
  ```

- ## Renomear a lista

  `PUT`
  `/list/rename` <br />
  `Parâmetros` :

  ```
      - boardId
      - listId 
	  - título
  ```

- ## Excluir a lista

  `PUT`
  `/list/remove` <br />
  `Parâmetros` :

  ```
  	- boardId
  	- listId 
  ```