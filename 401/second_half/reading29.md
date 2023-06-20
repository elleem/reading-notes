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

be sure to use dunder str

be sure to `def permissions`

be sure to `def has_module_perms`--they can change stuff in the db if they are admins

additional `class MyAccountManager` to extend the `BaseUserManager`
  `def create_user` with the required fields to create a user, need to do the same for `def create_superuser`

  if not email raise an error

  normalize_email will lower() all the characters in an email. only available in the BaseUserManager class. 

  set_password is another method that can be used on the user object. 

  set up flags for superuser, including is_admin, is_staff, is_superuser

set an object to `MyAccountManager()`

Be sure to set a property in `settings.py` `AUTH_USER = 'account.Account'`  reference the app and the model

add to `admin.py`

don't forget to re-migrate and re-create the superuser.

### DjangoX

3. What is DjangoX and how does it complement or extend the functionality of Django? Provide an example use case for incorporating DjangoX in a project.

DjangoX is an open-source project on GitHub. 

A set of extensions and tools that complements and extends the functionality of Django. 

DjangoX simplifies and streamlines the development process by providing additional features and utilities on top of Django.

Allows for enhanced admin interface, additional field types, extensions for models and forms (custom form widgets). 