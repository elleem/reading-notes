## APIs
summarized from: https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design


### Things I Want to Know More About

### Questions

What does REST stand for?
Representational State Transfer, an architectural style for building distrubted systems

REST APIs are designed around a **resource**, ie any kind of object, data or service accessed by the client.

What is an identifier of a resource? Give an example.
A Uniform Resource Identifier that ids the resource, aka web address

What are the most common HTTP verbs?
GET, POST, PUT, PATCH, DELETE

What should the URIs be based on?
the resource should be based on nouns (not verbs)

Give an example of a good URI.
combines the processes for the pathway to the end goal or operation, such as "order" vs "create order"
consistently named
simple
use HATEOAS to enable navigation to related resources (Hypertext as the Engine of Application State)

What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?
Nope, imposes a load on the web server, you might want to use pre-computed data, and combine related information into bigger resources that can be retrieved with one request

What status code does a successful GET request return?
**200**

What status code does an unsuccessful GET request return?
**404**

What status code does a successful POST request return?
**201**

What status code does a successful DELETE request return?
**204**