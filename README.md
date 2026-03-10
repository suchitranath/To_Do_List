# Ex03 To-Do List using JavaScript
## Date: 3/13/2026
## Submitted by: Suchitra Nath (212223220112) BTECH IT

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
<html>
<head>
<title>To Do List</title>
<link rel="stylesheet" href="style.css">
</head>

<body>

<h2>My To Do List</h2>

<input type="text" id="task" placeholder="Enter a task">
<button onclick="addTask()">Add</button>

<ul id="list"></ul>

<script src="script.js"></script>

</body>
</html>
```
style.css
```
body{
font-family: Arial;
text-align: center;
background-color: #f2f2f2;
}

input{
padding:8px;
}

button{
padding:8px;
margin-left:5px;
}

li{
margin:10px;
}
```
script.jss
```
function addTask(){

let task = document.getElementById("task").value;

if(task === ""){
alert("Enter a task");
return;
}

let li = document.createElement("li");
li.textContent = task;

let btn = document.createElement("button");
btn.textContent = "Delete";

btn.onclick = function(){
li.remove();
}

li.appendChild(btn);

document.getElementById("list").appendChild(li);

document.getElementById("task").value = "";

}
```

## OUTPUT
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/6f8bc4d7-2c89-4c70-9b5c-ebc5b7c0217d" />


## RESULT
The program for creating To-do list using JavaScript is executed successfully.
