# todo-app

<!DOCTYPE html>
	<html>
	<head>
	<title>To-do app</title>
	</head>
	<body>
	<form id="todoForm">
	<h1>TodoList App:<h1>
	<input id="todoInput">
		<button type="button" onclick="todoList()">Add Item</button>
	</form>
	<ol id="todoList">
	</ol>
	</body>
	</html>
  
  
  function todoList()
{
    var item  = document.getElementById('todoInput').value
    var text = document.createTextNode(item)
    var newItem = document.createElement('li')
    newItem.appendChild(text)
    document.getElementById("todoList").appendChild(newItem)

   }
