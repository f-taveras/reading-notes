<sub>Think you might be in the wrong place? [Go home!](../README.md)</sub>


## What are the key differences between scraping static and dynamic websites?
### Static Websites
* __Content Delivery:__ The content is directly embedded into the HTML of the webpage and is served as-is from the server.
* __Scraping Method:__ Generally easier to scrape as the data can be obtained directly from the HTML source code using tools like BeautifulSoup in Python.
* __Technologies:__ Primarily consists of basic HTML, CSS, and possibly some JavaScript.
### Dynamic Websites
* __Content Delivery:__ The content is dynamically loaded using JavaScript. This means that the initial HTML document might not contain the actual data you're interested in.
* __Scraping Method:__ Requires tools that can execute JavaScript and wait for the content to be loaded, often necessitating the use of headless browsers or similar technologies.
* __Technologies:__ Extensively uses JavaScript and APIs to fetch and display content.

## Explain at least three techniques or best practices that can be employed to avoid getting blocked while scraping websites.
* __Respect Robots.txt:__ This file on websites indicates which parts of the site should not be accessed by crawlers. Respecting these rules can prevent a scraper from being blocked.
* __Rate Limiting:__ Rapid, repeated requests to a website can trigger anti-scraping measures. Implementing delays between requests can reduce the likelihood of being detected and blocked.
* __User-Agent Rotation:__ Websites can block scrapers that use a single, identifiable user-agent. Rotating between different user-agent strings can help avoid detection.
* __IP Rotation:__ Using different IP addresses for scraping requests can prevent IP-based blocking. This can be achieved through proxies or VPN services.
* __Headers and Session Management:__ Mimicking a real user's browser session by managing cookies and using appropriate HTTP headers can reduce the chances of being blocked.

## What is Playwright, and how does it assist in web scraping tasks? Provide an example of a use case where Playwright would be particularly beneficial.

### What is Playwright?
Playwright is a Node library to automate the Chromium, WebKit, and Firefox browsers. It allows for the automation of web browser interactions, including those on dynamic websites.
* __Use Case in Web Scraping:__
Particularly beneficial for dynamic websites where content is loaded asynchronously via JavaScript. Playwright can wait for these elements to load before scraping, making it effective for sites with heavy client-side rendering.
* __Example Use Case:__

Scraping a single-page application __(SPA)__ like a modern e-commerce site, where product listings and prices are loaded dynamically in response to user actions. Playwright can simulate user interactions like scrolling, clicking on dropdowns, or filling out forms to ensure that all necessary content is loaded for scraping.

## Describe the purpose of using Xpath in web scraping, and provide an example of an Xpath expression to select a specific HTML element from a webpage.


* __Purpose of XPath:__
XPath is a language used for navigating through elements and attributes in an XML document. In web scraping, it's used to select specific HTML elements from a webpage.
* __Example XPath Expression:__
    - To select an element by its ID, you might use: `//*[@id='elementID']`
This XPath expression selects any element __(*)__ with the specified ID `(@id='elementID')`.

Using XPath allows for precise and flexible selection of HTML elements, which is particularly useful when dealing with complex and nested webpage structures.

<sub>Information modeled using ChatGPT</sub>