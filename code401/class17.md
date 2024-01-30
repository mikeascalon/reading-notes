# Reading Notes

What are the key differences between scraping static and dynamic websites?

**Static Websites**:

1.Static websites have all their content present in the initial HTML when the page loads.
2.There is no need for additional JavaScript execution to retrieve data.
3.Web scraping libraries like BeautifulSoup and lxml can be used to parse the HTML and extract data.
4.Data extraction from static websites is straightforward and does not require browser automation.

**Dynamic Websites:**

1.Dynamic websites load or update content after the initial HTML load using JavaScript.
2.To extract data from dynamic websites, you must execute internal JavaScript in the page context.
3.Libraries like BeautifulSoup alone are insufficient because they do not execute JavaScript, resulting in incomplete or incorrect data extraction.
4.Various techniques can be employed to scrape dynamic websites, including Selenium, Pyppeteer, Playwright, and Web Scraping API.
5.Selenium is a popular choice that allows communication with different web browsers using a webdriver.
6.Pyppeteer is a Python port of Puppeteer, a headless Chrome automation library.
7.Playwright is an extended version of Puppeteer that supports Chromium, Firefox, and Webkit.
8.Web Scraping API, such as ScrapingAnt, provides a simpler way to scrape dynamic websites by handling headless browser execution and proxies in the cloud.

Explain at least three techniques or best practices that can be employed to avoid getting blocked while scraping websites.

**Human copy-and-paste**
* The simplest form of web scraping is manually copying and pasting data from a web page into a text file or spreadsheet. Sometimes even the best web-scraping technology cannot replace a human's manual examination and copy-and-paste, and sometimes this may be the only workable solution when the websites for scraping explicitly set up barriers to prevent machine automation.

**Text pattern matching**
* A simple yet powerful approach to extract information from web pages can be based on the UNIX grep command or regular expression-matching facilities of programming languages (for instance Perl or Python).

**HTTP programming**
* Static and dynamic web pages can be retrieved by posting HTTP requests to the remote web server using socket programming.

What is Playwright, and how does it assist in web scraping tasks? Provide an example of a use case where Playwright would be particularly beneficial.


Playwright is an open-source automation library for browsers that allows developers to control web browsers programmatically. It was developed by Microsoft and provides a high-level, cross-browser API for automating tasks in web applications. Playwright supports multiple browsers, including Chromium, Firefox, and WebKit, making it a versatile tool for web automation and scraping tasks.

**Headless Browsing**: Playwright can run browsers in headless mode, which means the browser runs without a graphical user interface. This is particularly useful for web scraping because it allows you to interact with web pages, execute JavaScript, and extract data without the need for a visible browser window.

Describe the purpose of using Xpath in web scraping, and provide an example of an Xpath expression to select a specific HTML element from a webpage.

The primary purpose of using XPath in web scraping is to locate and target elements based on their position and structure within the document, making it an essential tool for data extraction.

Suppose you want to select all the hyperlinks (`<a>` tags) within a specific section of a webpage, say a section with the ID news-section.

The XPath expression for this would be:

```python
//div[@id='news-section']//a

```

Here's what this expression means:

// : Selects nodes from the current node that match the selection no matter where they are.

div[@id='news-section'] : Finds a `<div>` element with an ID of news-section.

//a : Within that `<div>`, selects all the `<a>` elements (hyperlinks).

## Resources

[Scrape a Dynamic Website with Python](https://scrapingant.com/blog/scrape-dynamic-website-with-python)

[Web scraping](https://en.wikipedia.org/wiki/Web_scraping)

[Playwright XPath Selectors](https://www.programsbuzz.com/article/playwright-xpath-selectors)

[Xpath cheatshee](https://devhints.io/xpath)

[Python Playwright Tutorial For Beginners](https://www.youtube.com/watch?v=yp1o9biMMWU)

[ChatGPT](https://chat.openai.com/)
