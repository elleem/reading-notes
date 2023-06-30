## Permissions and Postgresql

#### Things I Want to Know More About


### DRF Permissions

1. What are the key components and purpose of Django Rest Framework (DRF) permissions, and how do they help in securing an API?

determines whether a request should be granted or denied access for `request.user` or `request.auth`, especially in the case of `IsAuthenticated` users. 

Determined as a list of permissions classes, an exception is raised if a permissions check fails.

Also determined by object-level permissioning, usually in the model. 

You can set up these for the API: `AllowAny`, `IsAuthenticated`, `IsAdminUser`, `IsAuthenticatedOrReadOnly`

You can also set up custom permissions. 

### Review of SQL Prework

2. In SQL, what is the purpose of the SELECT statement, and how would you use it to retrieve all columns from a table called ‘employees’?

SELECT [stuff you want to select] FROM [table that it is in]; 
* splat = the whole table short cut

Sounds like you are asking me `SELECT * FROM employees;`

### Classy Django REST

### DRF Generic Views

3. Can you explain the role of DRF Generic Views and provide examples of their usage in building a RESTful API?

The generic views provided by REST framework allow you to quickly and simply build API views that map closely to your database models.

But you have the flexiblity to use the regular APIView class or reuse the mixins and base classes used by the generic views.

We employeed these in our last lab with `ListAPIView`, `RetrieveAPIView`, `CreateAPIView`. 
