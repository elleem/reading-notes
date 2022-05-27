## Local Storage

### Things I Want to Learn More About

### Past, Present, and Future of Local Storage for Web Applications

<p> Cookies: slow down apps, send unencrypted data over the web, limited to 4KB of data </p>
<p> You need a lot of space on the client, beyond the page refresh, and isn't transmitted to the server. </p>
<p> userData allows 65 KB per domain, 640 KB if trusted. </p>
<p> Gears used to be able to access SQL to save unlimited data. </p>
<p> HTML5 storage--stores key/value pairs locally, like cookies, persists after you navigate away from the page, available when 3rd party plugins are not. </p>
<p> Use modernizer to detect local storage. </p>
<p> Store data using named keys (stored in strings). If you are using anything else, then you will need to use other functions. </p>
<p> localStorage is an object and it be treated as an array. Instead of "getItem" write []</p>
<p> You can trap a local storage event via setItem, removeItem, clear and <em>something actually </em> changes. </p>
<p> 5 MB how much each storage space origin gets by default (strings), quota_exceeded_err, cannot get more storage space. </p> 
<p> Able to save progress locally via localStorage object, then use a resume object in this example. </p>
<p> Data as strings means that you will have to coerce it yourself when you retrieve it, so you may have to construct a boolean in some functions. </p>
<p> UMMMM. I feel like this article just referenced the first iphone I ever bought...</p>
<p> Index database API uses an object store, which shares many concepts with a SQL db, but without a sturctured query language. </p>


