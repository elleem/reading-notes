## Django REST Framework & Docker

#### Things I Want to Know More About


### Beginner's Guide to Docker

1. What are the key components of a Docker container, and how do they help streamline the development and deployment of applications?

isolates and run entire applications, no more venv, implements Linux containers

everyone can use the same development environment.

virtual environments are big and slow, like a single family home vs docker which is like an apartment.

an image is a snapshot in time of what a project contains, a container is running an instance of an image.

- A Dockerfile is the recipe for a cake
- An image is a snapshot of the recipe at a given time
- A docker-compose.yml says how to make the cake
- And the container is the actual, baked cake

Docker files are read from top to bottom. 

Each image is made up of one or more layers, with the base layer something like `alpine`.

This is called image layering and it exists for two main reasons. 

First, each image layer is immutable–unchanged–like a git commit. 

This helps ensure consistency when two developers build the same image. 

The second reason is performance. 

Docker caches the steps in a Dockerfile to speed up subsequent builds. 

When a change is made to a step, all steps following it will be executed from scratch.

### Django for APIs

2. Describe the primary steps involved in building a library website using Django, including essential components like models, views, and templates.

The most important takeaway is that Django creates websites containing webpages, while Django REST Framework creates web APIs which are a collection of URL endpoints containing available HTTP verbs that return JSON.

1. Install and create a django project. 
2. create an app.
3. create the model.
4. create a superuser
5. add items to db.
6. update views.py file
7. update urls.py
8. create templates
9. run tests

### Beginner's guide to Django REST Framework

3. Can you explain the primary differences between Django and Django REST framework?

Django is an Model-View-Controller or Template architecture. 

It also provides ORM, templates, and URL routing.

Django REST is an extension specifically for APIs. 

It follows Model View Serializer. 

It also provides tools for CRUD and you can return API data in various formats. 