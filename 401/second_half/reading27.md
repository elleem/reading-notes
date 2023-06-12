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

### Beginner's Guide to Django

3. Briefly outline the key components and workflow of a Django application, as discussed in the Beginner’s Guide to Django. How do these components interact with each other to create a functional web application?