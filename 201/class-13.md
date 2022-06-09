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


### JSON

<p> JavaScript Object Notation is a scheame-less text based representation of structured data this is based on key-value pairs and ordered lists. </p>
<p> used for information exchange between web clients and web servers. </p>
<p> a data structure, in local storage, can only store strings. you can stringify an object, can be saved in local storage. </p>
<p> If you don't save the information, it is isn't persistent. </p>
<p> Strings/text easy to send over the internet. </p>
<p> Generic data format with a minimal number of value types: strings, numbers, booleans, lists, objects, null. </p>
<p> Now sections of pages could be reloaded instead the full page. </p>
<p> You can create misshapen data. Only 1 number type. no date type. no comments. sometimes not the most concise data interchange format. </p>
<p> Use of a native parser method. </p>
<p> Utilites: Json formatter, json view, json beautifier, json converter. </p>

### Local Storage
<p> http is stateless, reset when you reopen. </p>
<p> local storage allows you to save information without forcing someone to sign up. </p>
<p> All you have to do is modify the localStorage (sessionStorage data only maintained until browser window closes) object in javascript, using setItem, getItem. </p>
<p> How to clear-- not provided for Chrome. </p>



