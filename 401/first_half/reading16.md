## Serverless Functions

#### Things I Want to Know More About


### What is Serverless Computing? 

1. What are the key characteristics of serverless computing, and how does it differ from traditional server-based architectures?

Cloud application development and execution model w/o managing servers, provider provisions the cloud infrastructure required to run your code, scales, provides routine infrastructure management and maintenance, such as OS updates, patches, security, capacity and system monitoring. 

It allows devs to focus on code and not infrastructure. 

Allows devs to use any language, you pay for execution only.


### venv--creation virtual environments

virtual environments w/ independent set of python packages installed in their site directories.

A virtual environment is a self-contained Python environment that allows devs to isolate project dependencies and avoid conflicts with other projects that may require different versions of the same package.

Once installed, you can use pip to install packages. 

Use requirements.txt to list all the required packages to share with other developers. 

### Vercel

2. How can one get started with Vercel, and what are the main steps involved in deploying a serverless function using Vercel?

Import an existing project via git and deploy. Continue developing with the normal development workflow, run locally, view the Vercel preview, ship your changes to production, once you push to your main branch.

Configure your project, using the built in development settings, or applying default routing rules based on the framework that was detected. Use json to configure additional rules. Configure API routes and environment variables. 

Assign a domain. Just like netlify or use a custom domain. 

Make changes with automatic deployments. They will be preview deployments on development branches, excluding production. You can set up vercel directly in the CLI. 

Add compute.  Client side rendering and server side rendering. 

Note: When a Serverless Function boots up from scratch, that is known as a cold boot. When it is re-used, we can say the function was warm.

Re-using a function means the underlying container that hosts it does not get discarded. State, such as temporary files, memory caches, sub-processes, is preserved

Monitor via logs and analytics. 

### http.server

When the request handler class gets the request, it looks at the method and knows which method to use. The method doesn't need any other information because it already knows everything about the request.

Finally, when the method finishes running, it sends a response back to the web page. This response is like a message telling the web page if it got what it asked for or not and sometimes appears as errors. 

Supporting POST requests is a little more work, because the base class does not parse the form data automatically. 

The send_header method adds header data to the HTTP response. It takes two arguments: the name of the header and the value.

http.server includes a built-in server for serving files from the local file system. Start it from the command line using the -m option for the Python interpreter.

### Requests

4. What is the Requests library in Python, and how can it be used to interact with APIs by sending HTTP requests? Can you provide an example of a basic GET request using the Requests library?

A library that you must install that allows devs to send requests in Python and makes it easy to interact with APIs. 

`import requests`

`r = requests.get('https://api.github.com/events')`

`r = requests.post('https://httpbin.org/post', data={'key': 'value'})`

`r = requests.put('https://httpbin.org/put', data={'key': 'value'})`

`r = requests.delete('https://httpbin.org/delete')`

`r = requests.head('https://httpbin.org/get')`

`r = requests.options('https://httpbin.org/get')`

### Python and APIs

3. What are APIs, and how can they be utilized in Python applications to access and manipulate data from external sources?

Application programming inteface, a communication layer that allows different systems to talk to each other w/o having to understand exactly what each does or the rules they follow. 

Make HTTP request to the API endpoints using `requests`. Still may have tokens. Returns the data to be parsed and used. 

Most APIs are still REST APIs. 

You can test some APIs directly fro the documentation page. 

Don't forget that ? helps you specify the params of the query if you need to cut down the data. such as `gender = female`

### What is Serverless? 

You are outsourcing servers to the cloud providers. 

Bare Metal is you are deploying, configuring, patches.

VM--resource optimization, but you still have to set up everything.

Containers--Docker, packaging code and dependencies, into one structure

Serverless--focused on business logic, FaaS, functions as a service, event driven architecture. Highly available, in multiple zones, and fault tolerant.

Cons--timeouts if your code does not execute within the window, latency. 

### Serverless Functions

Serverless Functions enable developers to write functions in JavaScript and other languages to handle user authentication, form submissions, database queries, custom Slack commands, and more.

Used via regions.

Enforce a maximum execution timeout. 

Leave the functions section open to see the calls in real time. 

### Effective Python Environments








