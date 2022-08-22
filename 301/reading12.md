## CRUD
summarized from: https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/ and https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw


### Things I Want to Know More About


### Questions

### Status codes based on REST methods

In your own words, describe what each group of status code represents:

100’s =
200’s =
300’s =
400’s =
500’s =
What is a status code 202?
What is a status code 308?
What code would you use if an update didn’t return data to a client?
What code would you use if a resource used to exist but no longer does?
What is the ‘Forbidden’ status code?

### Build a REST API with Node.js, Express, & MongoDB

Why do we need to pull our MongoDB database string out of our server and put it into our .env?
we will not use local host for deployment, also I'm trying to keep my password a secret!

What is middleware?
code that runs when the server gets a request, but before it is passed to our routes. 

What does app.use(express.json()) do?
allows the server to accept json as a body, as opposed to a GET element

What does the /:id mean in a route?
it makes it a parameter, which we can access by type `req.params.id` and allows access to what ever is created after the first slash for GET

What is the difference between PUT and PATCH?
patch updates only the elements that the subscriber updates, put updates all the information 

How do you make a default value in a schema?
use `default` as the key

What does a 500 error status code mean?
means there is an error on the server, the db had an error, the user/client does not have an error, any error in the 500 range means there is an error on the server.

What is the difference between a status 200 and a status 201?
201 means successfully created an object and is more specific, 200 means everything was successful

REST client extension via VSC