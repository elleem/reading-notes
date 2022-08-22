## CRUD
summarized from: https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/ and https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw


### Things I Want to Know More About


### Questions

### Status codes based on REST methods

In your own words, describe what each group of status code represents:

100’s = informational status codes that tell the client that the header part of the request has been received and the server will try to comply with a transmission demand of the client. 

200’s = success codes, request was accepted and meets the validation requirements at the time of sending

300’s = redirection codes, the resource they are requesting isn't available at the expected location

400’s = client error codes, invalid requests sent to a server, timeouts, wrong URI, authentication is missing

500’s = server error codes, indicate problems with overwelmed servers, unreachable servers

What is a status code 202?
asynchronous processing of a request, req accepted and will be processed in the future

What is a status code 308?
permanent redirect, tells the client to use another URL to access the resource

What code would you use if an update didn’t return data to a client?
204 no content

What code would you use if a resource used to exist but no longer does?
308, permanent redirect

What is the ‘Forbidden’ status code?
403

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