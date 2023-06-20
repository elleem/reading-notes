## Django Custom User

#### Things I Want to Know More About


### Django User Model




1. What are the key benefits of using a Django Custom User Model, and how does it differ from the default Django User Model?

it extends the model and allows you to control more than what the generic model provides, including allowing users to login with their emails instead of user names. 

build a custom user model will allow it to fit your needs.

Use the email, instead of a username. 


2. Explain the process of creating and implementing a Custom User Model in Django, including the necessary changes to settings.py and the required model fields.

  coding with mitch blog course

Deletes the database, so that there will be a clean slate. delete the numbered migrations. Run the server to re-generate the database. 

`python manage.py startapp account` which creates a custom app, be sure to add in `settings.py`

go into `models.py` and `from django.contrib.auth.models import AbstractBaseUser, BaseUserManager` classes that you can use to extend the generic django user model. 

```python
class Account(AbstractBaseUser):
    email              *models.EmailField(verbose_name = 'email', max_length=60, unique=True)
    username           *models.CharField(max_length=30, unique = True)
```
set all required fields, above also set up the flags for database specific fields such as `is_superuser`

`USERNAME_FIELD = 'email'`

`REQUIRED_FIELDS = ['username']`


### DjangoX

3. What is DjangoX and how does it complement or extend the functionality of Django? Provide an example use case for incorporating DjangoX in a project.

