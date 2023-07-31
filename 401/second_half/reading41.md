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

### Next.js 10 is here

### Next.js Static File Serving

3. How does Next.js handle static file serving? Discuss the default folder structure for storing static assets and explain how to reference them in a Next.js application.



