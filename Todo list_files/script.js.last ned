// add global variables
const inputElement = document.getElementById("task-input");
const addTaskButton = document.querySelector("#add-task");
const taskList = document.querySelector("#task-list");

// add event listener to button with click and function name
addTaskButton.addEventListener("click", addTask)
// press ENTER to add task to list
document.addEventListener("keydown", function(event) {
    if (event.key === "Enter") {
        addTask();
    }
})
// create function ORDER IS IMPORTANT
function addTask() {
// store value/contents of input in "task" variable
    const task = inputElement.value 
// error message IF no input
    if (task === "") {
        alert("Please enter a task!")
// return: breaks out of function and does NOT run the rest of it
        return;
    }
// clear text content of input box after adding task
    inputElement.value = "";
// create list element that didnt exist before
    const listItem = document.createElement("li");
// create list item class
    listItem.className = "task-list-item";
// create paragraph
    const textElement = document.createElement("p");
// target paragraph, give it content that is stored inside "task" variable
    textElement.textContent = task;
// create checkbox, make line-through if checked and not if not
    const checkbox = document.createElement("input");
    checkbox.type = "checkbox";
    checkbox.className = "task-checkbox";
    checkbox.addEventListener("change", function () {
        if (checkbox.checked) {
            textElement.style.textDecoration = "line-through";
        } else {
            textElement.style.textDecoration = "none";
            textElement.style.color = ""
        }
    });
    
// append to actually appear in html
    listItem.appendChild(checkbox);
    listItem.appendChild(textElement);
    taskList.appendChild(listItem);
// delete button
    const deleteButton = document.createElement("button")
    deleteButton.textContent = "Delete"
    deleteButton.addEventListener("click", function () {
        listItem.remove()
    });
    deleteButton.className = "delete-button";
    listItem.appendChild(deleteButton);
}