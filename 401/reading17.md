## Web Scraping

#### Things I Want to Know More About


### Scrape a Dynamic Website with Python

1. What are the key differences between scraping static and dynamic websites?

A dynamic website can update or load content after the initial HTML load, increasing page load speed and prevent reloading each time you load a page. 

Static sites load all requested information upon page load. 

We need the HTML to run in the browser to see the correct values and then capture the values programmatically. 

four different ways to execute dynamic website's Javascript and provide valid data for an HTML parser: 

Selenium, Pyppeteer, Playwright, and Web Scraping API.

- `pip install selenium`, uses a special connector--webdriver. 
- define and setup Chrome path variable
- define and setup Chrome webdriver path variable
- define browser launch arguments (to use headless mode, proxy, etc.)
- instantiate a webdriver with defined above options
- load a webpage via instantiated webdriver

Puppeteer is a high-level API to control headless Chrome, so it allows you to automate actions you're doing manually with the browser: copy page's text, download images, save page

Also `pip install pyppeteer` and playwrite.

ScrapingAnt web scraping API provides an ability to scrape dynamic websites with only a single API call.

`pip install scrapingant-client`


### What is Web Scraping?

data scraping used for the automated extraction of data from websites. 

usually with a bot or web crawler. an example would be contact scraping. 

Newer forms monitor the JSON. 

The legal section was interesting. 

### How to Scrape websites without getting blocked

2. Explain at least three techniques or best practices that can be employed to avoid getting blocked while scraping websites.

Follow the robot.txt file for scraping rules. 

Crawl slowly (sleep calls in b/n requests, add some delays, choose the lowest number of concurrent requests possible, auto-throttle)

Do not follow the same crawling pattern (add random clicks, mousing, and actions)

Make requests thru proxies, rotate as needed using VPNs, free proxies

Rotate users agents, and HTTP request headers between requests--what? you can pretend to be a google bot? 

Use a headless browser, such as Pyppeteer, Selenium or Playwrite. 

Beware of honey pot traps (invisible links to catch bots)

Check if site is changing layouts. 

avoid scraping behind a login (you have to send cookies w/ ea request to view the page)

use captcha solving services

### Login and Scrape Data with Playwright and Python

3. What is Playwright, and how does it assist in web scraping tasks? Provide an example of a use case where Playwright would be particularly beneficial.

Playwright is an open-source automation library for web testing and scraping tasks. It provides a high-level API to control web browsers, including Chromium, Firefox, and WebKit. Playwright allows developers to write automated tests and perform web scraping tasks with a single, consistent API that works across multiple browsers.

Price scraping

`from playwrite.sync_api import sync-playwrite`

`with sync_playwrite() as p:`

  `brower = p.chromium.launch(headless=False, slow_mo= 50)`

  `page = browser.new_page()`

  `page.goto('site address')`

  query selector to use CSS, load the page, capture parts of the HTML and send to beautiful soup

  easy way is using `page.innner.html()`

  using the chrome dev tools to find the tags that he needs. 

  `page.is_visible()`

### Python Playwrite Tutorial for Beginners

automation of web browers



### Beautiful Soup

### Playwrite XPath Selectors

4. Describe the purpose of using Xpath in web scraping, and provide an example of an Xpath expression to select a specific HTML element from a webpage.

Xpath is a query language which scrapes the web, navigating the document structure and extracts data from HTML elements. 

`//h1`

`//` selects any element in the document that matches the following criteria

`h1` targets `h1` elements specifically






