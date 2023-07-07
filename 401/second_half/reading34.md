## API Deployment

#### Things I Want to Know More About


### Django Settings Best Practices

1. What are the key principles to follow when organizing and configuring Django settings for a project, according to the “Django Settings Best Practices” reading?

1. separate settings for different environments
2. use environment variables
3. keep sensitive data out of version control
4. share default configurations with devs
5. use modules
6. read environment variables
7. use recognizable names

### White Noise

2. How does the White Noise library contribute to the efficient serving of static files in a Django application, and what are the steps to integrate it into a project?

It is a middleware that serves static assets (CSS, JS and images) in Django applications for production servers. The compression reduces the bandwidth required for CSS and JS. 

the server needs to examine the `Accept-Encoding` header of the request to determine which compression formats are supported, and return an appropriate `Vary` header so that intermediate caches know to do the same. 
 
install with `pip install whitenoise`

### CORS

3. What is the purpose of Cross-Origin Resource Sharing (CORS) in web applications, and how can it be implemented and configured in a Django project to control access to resources?

It is a mechanism that allows restricted resources (APIs) on a web page to be accessed from another domain outside the domain from which the first resource was served.

Determines if it is safe to allow a cross-origin request. 

The body guard!

`pip install django-cors-headers`

add to `settings.py`

add to `INSTALLED_APS`

add to `MIDDLEWARE`

configure CORS settings `CORS_ORIGIN_ALLOW_ALL = False`, the provide `CORS_ORIGIN_WHITELIST`