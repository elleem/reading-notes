## Authentication and Production Server

#### Things I Want to Know More About


### JSON Web Tokens

1. What is the primary purpose of JSON Web Tokens (JWTs) and how do they work in terms of encoding and decoding data?

JWTs verify the integrity of the claims contained within. The signature certifies only the private party holding the key is the one that signed it. 

Allow for authorization and information exchange. 

Allowing authenticated users to access information permitted via the token. SSO 

Allows you to authenticate senders, ensures that via header/payload you can verify the content hasn't been tampered with. 

3 parts: header, payload, signature.

  Header = type of token and signing algorithm

  Payload = contains claims, including registered, public, and private claims. 

  Signature = to create signature take the encoded header and payload, secret, and the alogrithm specified in the header and sign that. 

The output is three Base64-URLs that can be passed in HTML, HTTP environments. 

JSON tokens: when a user logs their credentials a web token will be returned. 

### DRF JWT Authenication

2. How does JWT Authentication integrate with Django REST Framework to secure API endpoints, and what are the key components involved in this process?

By passing the token with each request, exchanges the username/password for an access token and refresh token. 

Send a post request, then you get the access/ refresh tokens. 

You can protect your API endpoints by adding the access token in the header of all requests. 

### Django Runserver is Not Your Production Server

3. Why is Django’s built-in runserver not suitable for production environments, and what are some alternative server options that should be considered for deploying a Django application?

It has not gone through security audits or performance (slow) tests. 

Nginx, Gunicorn

### JWT with DRF

allows verification of secrets

install djangorestframework_simplejwt

update `settings.py` with `REST_FRAMEWORK = {}` add in permissions and authentication classes

update `urls.py` need to allow users to get the token by creating the endpoints, via `urlpatterns` 

need 2 urls one to get the token, one to refresh the token

postman to test APIs

creates `send.py` import request

able to run the file in the terminal





