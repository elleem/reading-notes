## Authentication
summarized from: https://www.npr.org/sections/money/2014/10/21/357629765/when-women-stopped-coding and https://informationisbeautiful.net/visualizations/diversity-in-tech/ and https://www.usatoday.com/story/tech/columnist/2015/07/21/why-diversity-matters-your-tech-company/30419871/


### Things I Want to Know More About


### Questions

### What is OAuth

What is OAuth?
secure, third-party, user-agent delegated authorization that allows authentical access to server/services assets

Give an example of what using OAuth would look like.
using your Google authentication to login into other websites like Heroku

How does OAuth work? What are the steps that it takes to authenticate the user?
like a valet temporarily parking a car, it allows the user via an authentication provider to give a limited access token for authorization, 

What is OpenID?
OpenID is about authentication and eventually became an authetentication layer for OAuth


### Authorization and Authentication Flows

What is the difference between authorization and authentication?
authorization: verifying who a user is
authentication: verifying what they have access to

What is Authorization Code Flow?
it exchanges an authorization code of a token

What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?
The PKCE-enhanced Authorization Code Flow introduces a secret created by the calling application that can be verified by the authorization server; this secret is called the Code Verifier. this is very important for native and single-page apps because they cannot securely store a Client Secret a) because their entire source is availble on the browser, and b) cannot securely store a client secret.

What is Implicit Flow with Form Post?
allows public clients, or applications that cannot store client secrets

What is Client Credentials Flow?
machine to machine application, such as daemons, or services running on your back-end the system authenticates and authorizes the app, rather than the user. 

What is Device Authorization Flow?
Uses a link for a pc, or phone, so that input-constrained devices, can authorize the device

What is Resource Owner Password Flow?
highly trusted applications can use the flow to request users provide credentials using an interactive form
