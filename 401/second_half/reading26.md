## Intro to Django

#### Things I Want to Know More About


### Getting Started with Django

What are the key components of the Django framework, and how do they contribute to building a web application?

a web development/framework app that is free and open source, site maps, user authentication, content administration, RSS feeds, scalable, allows Python code instead of SQL queries. Handles middleware, forms, and models for the structure and behavior of data in your application. Additionally, allows admin login. 

### How Django Works Behind the Scences

Pretty sweet open source project. 

### What is Django

`python -m pip install Django`

Explain the role of Django’s MTV (Model-View-Template) architecture and how it handles a typical web request-response cycle.

**M** defines structure and behavior of data in your app, representing db tables and handling db interactions.  1st step in the response cycle

**V** handles logic of your app, receive requests, process data, return responses

**T** define the presentation layer of your application, receives data from views and uses it generate dynmic web pages, display info, loop through lists, perform conditional rendering, apply formatting

Overall allows for code reusability and modular development. 

### What is Tailwind CSS? 

What is the purpose of Tailwind CSS, and how does it differ from Bootstrap CSS?

framework so that you don't have to write custom CSS

use classes to control the layout, color, etc. 

write less custom CSS, keep CSS files smaller, no inventing class names, make safer changes. 

Does not offer fully styled component like Bootstrap. instead it offers utility classes so that you can create your own reusable components, and offers more flexibility. 

`npm install -D tailwindcss`