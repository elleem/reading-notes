## Django Models

#### Things I Want to Know More About


### Using Models

1. Explain the purpose and basic structure of Django models. How do they help in creating and managing database schema in a Django application?

Models define the structures of the stored data, including field types, maybe max size, default values, selection list options, help text for documentation, label text for forms. Independent of the underlying database. Django communicates with it. 

Models represent each object or group of related information. You can define relationships, `OneToOneField` one to many `ForeignKey` and `ManyToManyField`. 

Relationships can have multiplicities. 

based in the models.py

Can have an arbitrary number of fields, of any type, each one represents a column of data that we want to store in one of our database tables. Each row consists of one of each field value. 

The field name is used to refer to it in queries and templates. Fields also have a label. 

Meta data: controls the default ordering of the records. 

`class Meta:`
    `ordering = ['-my_field_name']`

**Minimally, in every model you should define the standard Python class method `__str__()` to return a human-readable string for each object.**

Once you create model classes, you can CRUD, run queries. 

### Django Admin

2. Describe the primary features and functionality of the Django Admin interface. How can it be customized to suit the specific needs of a project?

use your models to build a site area that you can use to create, view, update, and delete records. Useful for testing, and managing data in production. Allows a superuser. 

Start by registering the models. 

`admin.py `

`from django.contrib import admin`

then import the models. 

customize permissions in `manage.py`


- Each model has a list of individual records, identified by the string created with the model's __str__() method, and linked to detail views/forms for editing. By default, this view has an action menu at the top that you can use to perform bulk delete operations on records.

- The model detail record forms for editing and adding records contain all the fields in the model, laid out vertically in their declaration order.

- Further customize this by adding list views, detail views. 

### Beginner's Guide to Django

3. Briefly outline the key components and workflow of a Django application, as discussed in the Beginner’s Guide to Django. How do these components interact with each other to create a functional web application?