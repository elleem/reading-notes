## Django CRUD and Forms

#### Things I Want to Know More About


### Django Forms

1. How do Django Forms facilitate user input handling, and what are some key components of creating a form using the Django framework?

Forms collect information from fields to transmit to the server, includes text, boxes, checkboxes, radio buttons, everything a user can manipulate. 

Forms POST. Created via `<form>` tag. Looks similar to setting up a model, uses many similar model field classes, such as `CharField`. Form, url, view. 

Forms include a lot of additional interaction such as validation and data processing, handle erros, handle data when it is submitted, and then confirm with the user. 

  1. display the default the first time the form is requested
  2. receive data from a submit request and bind it to the form
  3. clean and validate the data
  4. if any data is invalid, re-display with any error messages, and correct data
  5. once all actions are complete, redirect user to another page




2. Explain the purpose of Django Templates in web development and describe how template inheritance can be utilized to improve code reusability and maintainability.

Allows for more generic editing views. 

Seperation of concerns: separate the presentation layer form the underlying business logic

code reuse and maintainability, so that you can have a common layout for multiple webpages, starting with header, footer, and other elements, then can override with the children. 