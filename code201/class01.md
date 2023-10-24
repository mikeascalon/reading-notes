# Reading - Notes Class 1

1.Compose a short poem describing how HTTP sends data between computers.

* HTTP sends data between the client makes a request to the server. As ther server recieve the request, It calculates and responses to the client.

2.Describe how HTML, CSS, and JS files are “parsed” in the browser.

* HTML is like the skeleton of the webpage. It gives the structure of page in plain text. CSS will style the pafe from the background color, alignment and font  size. Finally the JS files will make the page interactive and dynamic behavior.

3.How can you find images to add to a Website?

* You can google and save it as a .jpg file. To add it a website just need to save it on the same directory. Then add on you .html file.

4.How do you create a String vs a Number in JavaScript?

* To create a string, you can use either single quotes (') or double quotes (") around the text you want to represent as a string

* To create a number in JavaScript, you can use numeric literals without quotes.

5.What is a Variable and why are they important in JavaScript?

* A variable in JavaScript is a named storage location that holds data. It acts as a container for values, such as numbers, strings, objects, or functions.

## Introduction to HTML

1.What is an HTML attribute?

* HTML attribute is a characteristic or property that is applied to an HTML element to provide additional information or modify the element's behavior. Attributes are used to define various aspects of an element, such as its appearance, behavior, and interaction. They are typically specified within the opening tag of an HTML element and are written as name-value pairs.

2.Describe the Anatomy of an HTMl element.

* The opening tag: This consists of the name of the element (in this example, p for paragraph), wrapped in opening and closing angle brackets. This opening tag marks where the element begins or starts to take effect. In this example, it precedes the start of the paragraph text.
* The content: This is the content of the element. In this example, it is the paragraph text.
* The closing tag: This is the same as the opening tag, except that it includes a forward slash before the element name. This marks where the element ends. Failing to include a closing tag is a common beginner error that can produce peculiar results.

3.What is the Difference between `<article>` and `<section>` element tags?

* The main difference between `<article>` and `<section>` elements is their purpose and how they represent content. Use the `<article>` element for standalone, distributable content like articles or blog posts. Use the `<section>` element to group related content thematically within a document, even if that content isn't intended to stand alone. Properly using these elements enhances the semantic structure and accessibility of your web page, making it more understandable to both users and search engines.

4.What Elements does a “typical” website include?.

* `<main>` is for content unique to this page. Use `<main>` only once per page, and put it directly inside `<body>`. Ideally this shouldn't be nested within other elements.

* `<article>` encloses a block of related content that makes sense on its own without the rest of the page (e.g., a single blog post).

* `<section>` is similar to `<article>`, but it is more for grouping together a single part of the page that constitutes one single piece of functionality (e.g., a mini map, or a set of article headlines and summaries), or a theme. It's considered best practice to begin each section with a heading; also note that you can break `<article>`s up into different `<section>`s, or `<section>`s up into different `<article>`s, depending on the context.

* `<aside>` contains content that is not directly related to the main content but can provide additional information indirectly related to it (glossary entries, author biography, related links, etc.).

* `<header>` represents a group of introductory content. If it is a child of `<body>` it defines the global header of a webpage, but if it's a child of an `<article>` or `<section>` it defines a specific header for that section (try not to confuse this with titles and headings).

* `<nav>` contains the main navigation functionality for the page. Secondary links, etc., would not go in the navigation.

* `<footer>` represents a group of end content for a page.

5.How does metadata influence Search Engine Optimization?

* Metadata plays a significant role in Search Engine Optimization (SEO) by providing information to search engines about the content and structure of web pages. It helps search engines understand the relevance and quality of a web page's content, making it more likely to appear in search engine results pages (SERPs).

6.How is the `<meta>` HTML tag used when specifying metadata?

* Metadata is data that describes data, and HTML has an "official" way of adding metadata to a document — the `<meta>` element.

## Starting a Website

1.What is the first step to designing a Website?

* To know what you want to accomplish.

2.What is the most important question to answer when designing a Website?

* What exactly do I want to accomplish?
* How will a website help me reach my goals?
* What needs to be done, and in what order, to reach my goals?

## Semantics

1.Why should you use an `<h1>` element over a `<span>` element to display a top level heading?

* using semantic HTML tags like `<h1>` for top-level headings provides a structured, meaningful, and accessible foundation for your web content.

* The `<span>` element is often used when you need to target a specific section of text within a larger context and do not want to introduce a new block-level element like a `<div>`, which would affect the layout.

2.What are the benefits of using semantic tags in our HTML?

* Search engines will consider its contents as important keywords to influence the page's search rankings (see SEO)

* Screen readers can use it as a signpost to help visually impaired users navigate a page

* Finding blocks of meaningful code is significantly easier than searching through endless divs with or without semantic or namespaced classes

* Suggests to the developer the type of data that will be populated

* Semantic naming mirrors proper custom element/component naming

## Things I want to know more about

1.Understanding more indepth about Meta Data.

### Resourses

[Getting started with HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started)

[Document and website structure](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Document_and_website_structure)

[Starting a Website](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/Design_and_accessibility/Thinking_before_coding)

[Chat GPT](https://openai.com/chatgpt)
