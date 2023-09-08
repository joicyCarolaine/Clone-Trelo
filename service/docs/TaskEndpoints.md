- ## Criar uma nova tarefa

  `POST`
  `/task` <br />
  `Parâmetros` :

  ```
  	- boardId
  	- listId
  	- tarefa (342(id da tarefa) : {id, título})
  	- taskIds (array de IDs de tarefas : ["123", "321", "342"])
  ```

- ## Reordenar uma tarefa (na mesma lista)

  `PUT`
  `/task-reorder` <br />
  `Parâmetros` :

  ```
  	- boardId
  	- listId
  	- taskIds
  ```

- ## Alternar uma tarefa entre listas

  `PUT`
  `/task-switch` <br />
  `Parâmetros` :

  ```
  	- boardId
  	- lists (atualizando todas as listas esperadas em um array ["123" : {...}, "321" : {...}])
  ```

- ## Atualizar uma tarefa

  `PUT`
  `/task-update` <br />
  `Parâmetros` :

  ```
      - boardId
      - taskId
	  - propriedade (título, descrição, anexos, atribuições, comentários, etiquetas)
	  - dados (dados da propriedade)
  ```
