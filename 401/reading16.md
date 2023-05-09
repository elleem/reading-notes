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

### Requests

4. What is the Requests library in Python, and how can it be used to interact with APIs by sending HTTP requests? Can you provide an example of a basic GET request using the Requests library?

### Python and APIs

3. What are APIs, and how can they be utilized in Python applications to access and manipulate data from external sources?

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








