## React 4

#### Things I Want to Know More About

### Next.js Dynamic Routes

1. Explain the concept of dynamic routes in Next.js and how they differ from static routes.

The page path depends on external data, but you can statically generate pages with paths that depend on external data = dynamic URLs.

For example you want to access blog posts, each post will have an `[id].js` 

`[]` indicating a dynamic route

use an async functon `getStaticPaths()` which runs at build time

use `getAllPostIds()` to return an array of objects to map through, ea obj must have a params key and contain an obj w/ id key, otherwise `getStaticPaths()` will fail

`npm install remark remark-html`

`npm install date-fns`

  `<Link href={`/posts/${id}`}>{title}</Link>`

I could see how this is all information that would fit in perfectly for the list of locations in the Overview page we built. 

### Next.js Deployment

2. Describe the process of deploying a Next.js application. What are the key steps involved, and what are some deployment platforms you can use?

DPS= Develop, Preview, Ship (write your code, **push changes to a branch on github to create a preview**, merge to main)

Vercel or your own hosting provider (that supports Node.js)

- import your repo into Vercel (allows custom domains, environment variables, auto HTTPS)

### Next.js 10 is here

10/27/2020 Next.js 10 launched

built-in image component and optimization, even outside images. via importing `Image`

improved language support

analytics view is improved and robust, free for hobby plans

improved e-commerce functionality

`getStaticProps()` improved with FAST

ability to import third party css inside of React component, ability to use datepicker without needing to import CSS in `_app.js`

auto resolves `href` which likely I would not notice due to only knowing Next.js 10

blocking the fallback, first blog load is empty, but now the initial request is waited on for pre-rendering

### Next.js Static File Serving

3. How does Next.js handle static file serving? Discuss the default folder structure for storing static assets and explain how to reference them in a Next.js application.

Static files are served via the `public` folder (I learned this early on when we were discussing which files should be deleted, because I looked this up)

`public` folder is like `(/)`  

also useful for `robots.txt` and `favico.ico`

do not name a `public` folder in `pages/`

I researched this further and discovered that for project organization you can create subdirectories. 

`static/` is from 9.1 next.js

