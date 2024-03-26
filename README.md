# CODSOFT INTERNSHIP TO-DO-LIST WEB APPLICATION
# Document Structure:

* The <!DOCTYPE html> declaration specifies the document type and version of HTML being used.
* The <html> element is the root element of the document, and lang="en" attribute indicates that the content is in English.
# Head Section:

* The <head> section contains metadata about the document, such as character encoding and viewport settings.
* Metadata helps browsers understand how to interpret and display the content of the webpage.
* In this code, the metadata includes charset, viewport settings, and the title of the webpage.
# External Stylesheet:

* The <link> tag imports an external stylesheet from Bootstrap CDN (Content Delivery Network).
* Bootstrap is a popular CSS framework that provides pre-designed styles and components for building responsive web applications.
# Body Section:

* The <body> element contains the visible content of the webpage.
# Container and Heading:

* The content is wrapped in a <div> element with the class container for styling purposes.
* The <h1> heading element with the class text-center mt-5 displays the title "To-Do List" at the center of the page.
# Form for Adding Tasks:

* A <form> element allows users to input task details such as task name, priority, due date, and category.
* Input fields (<input>, <select>) and labels (<label>) are used to collect task information.
* The form submits data to the "/add" endpoint using the POST method when the "Add Task" button is clicked.
# Task List:

* Below the form, a heading (<h2>) displays "Task List".
* A <table> element is used to display a list of tasks.
* Table headers (<thead>) define the columns: Task, Priority, Due Date, Category, and Actions.
* Table rows (<tr>) and cells (<td>) display task details fetched from the backend (e.g., task name, priority, due date, category).
* Action buttons within the last column allow users to complete or delete tasks by clicking on them. These buttons are linked to specific endpoints ("/complete/{{ task.id }}" and "/delete/{{ task.id }}").
# Template Rendering:

{% for task in tasks %} and {% endfor %} are template tags used by server-side templating engines (e.g., Jinja2) to loop through tasks retrieved from the backend and render them dynamically within the HTML template.
