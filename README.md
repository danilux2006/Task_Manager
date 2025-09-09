Team Project: JS Fundamentals + ES6+ with React 
This project is designed to help practice JavaScript Fundamentals (variables, functions) and 
ES6+ features (arrow functions, destructuring, spread/rest) in a collaborative React 
environment using GitHub for version control. 
Project Idea: Team Task Manager App 
A simple React app where users can add, view, and manage tasks. It provides opportunities 
to use JS fundamentals, ES6+ features, and team collaboration via GitHub. 
Core Features 
 Add Tasks – use variables and functions to manage state. 
 List Tasks – render tasks dynamically in React. 
 Mark Task as Complete – toggle state with a function. 
 Delete Task – use spread operator to remove items immutably. 
 Team Collaboration – each teammate adds one feature/logic via GitHub branches. 
JS Concepts Demonstrated 
 Variables & Functions – managing tasks (arrays, objects). 
 Arrow Functions – event handlers (onClick, onChange). 
 Destructuring – props and state values in components. 
 Spread/Rest – adding/removing tasks in arrays. 
Component Structure 
 App.jsx – Main entry point. 
 TaskForm.jsx – Input form for new tasks. 
 TaskList.jsx – Displays all tasks. 
 TaskItem.jsx – Each task with complete/delete buttons. 
Example Code Snippet 
// TaskList.jsx 
import React from "react"; 
const TaskList = ({ tasks, toggleComplete, deleteTask }) => { 
return ( 
<ul> 
{tasks.map(({ id, title, completed }) => ( 
<li key={id}> 
<span style={{ textDecoration: completed ? "line-through" : 
"none" }}> 
{title} 
</span> 
<button onClick={() => toggleComplete(id)}>✔️</button> 
<button onClick={() => deleteTask(id)}>❌</button> 
</li> 
))} 
</ul> 
); 
}; 
export default TaskList; 
GitHub Workflow 
 One person sets up React app (npx create-react-app team-task-manager). 
 Create a GitHub repo, push the starter code. 
 Each teammate works on a feature branch (e.g., feature/add-task, feature/delete-task). 
 Use Pull Requests for code reviews before merging.
