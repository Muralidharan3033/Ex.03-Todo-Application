# Ex03 To-Do List using JavaScript
## Date: 23.03.2025

## AIM
To create a To-do Application with all features using JavaScript.

## ALGORITHM
### STEP 1
Build the HTML structure (index.html).

### STEP 2
Style the App (style.css).

### STEP 3
Plan the features the To-Do App should have.

### STEP 4
Create a To-do application using Javascript.

### STEP 5
Add functionalities.

### STEP 6
Test the App.

### STEP 7
Open the HTML file in a browser to check layout and functionality.

### STEP 8
Fix styling issues and refine content placement.

### STEP 9
Deploy the website.

### STEP 10
Upload to GitHub Pages for free hosting.

## PROGRAM

index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Minimal Todo App</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>

  <h2>Todo List</h2>
  <input type="text" id="taskInput" placeholder="Add a task">
  <button onclick="addTask()">Add</button>
  <ul id="taskList"></ul>

  <script src="script.js"></script>
</body>
</html>

```

style.css
```
body {
  font-family: sans-serif;
  padding: 20px;
  max-width: 400px;
  margin: auto;
}

input {
  width: 70%;
  padding: 8px;
  font-size: 14px;
}

button {
  padding: 8px 12px;
  font-size: 14px;
  margin-left: 5px;
  cursor: pointer;
}

ul {
  list-style: none;
  padding: 0;
  margin-top: 20px;
}

li {
  padding: 6px 0;
  border-bottom: 1px solid #ddd;
  font-size: 16px;
  cursor: pointer;
}

.completed {
  text-decoration: line-through;
  color: #aaa;
}

```

script.js
```
function addTask() {
  const input = document.getElementById('taskInput');
  const text = input.value.trim();
  if (!text) return;

  const li = document.createElement('li');
  li.textContent = text;

  li.onclick = () => li.classList.toggle('completed');
  li.ondblclick = () => li.remove();

  document.getElementById('taskList').appendChild(li);
  input.value = '';
}

```


## OUTPUT
![Screenshot 2025-04-28 181339](https://github.com/user-attachments/assets/83689e54-f6d2-4254-8513-818f65c69b8e)


## RESULT
The program for creating To-do list using JavaScript is executed successfully.
