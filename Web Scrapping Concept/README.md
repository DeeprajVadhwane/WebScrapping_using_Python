# Introduction to Web Scraping

## 1. Introduction to Web Scraping

In today's world, we have tons of unstructured data/information (mostly web data) available freely. Sometimes the freely available data is easy to read and sometimes not. No matter how your data is available, web scraping is a very useful tool to transform unstructured data into structured data that is easier to read and analyze. In other words, web scraping is a way to collect, organize and analyze this enormous amount of data. So let us first understand what is web-scraping.

### When and Where Data Scientists/Analysts Use Web Scraping:

- **When:** When data is not readily available in a structured format (e.g., APIs, databases).
- **Where:** E-commerce, social media, news websites, financial sites, etc.

### Why Use Web Scraping?

- **Data Collection:** Gather large amounts of data from the web quickly and efficiently.
- **Automation:** Automate the process of data collection and updates.
- **Insights:** Derive insights from data that is not easily accessible through other means.

### Ethical and Legal Considerations:

- **Ethics:** Respecting website terms of service, avoiding overloading servers.
- **Legality:** Following the robots.txt file, understanding copyright laws.

### Common Web Scraping Tools:

- **Libraries:** Beautiful Soup, Scrapy, Selenium, Requests.
- **Comparison:** Use cases for each tool.

## 2. Basic HTML and CSS

### HTML Tree Structure

Before we look into the functionality provided by Beautiful Soup, let us first understand the HTML tree structure.

The root element in the document tree is the `<html>`, which can have parents, children, and siblings, determined by its position in the tree structure. To move among HTML elements, attributes, and text, you have to move among nodes in your tree structure.

### Content:

#### Basics of HTML:

- **HTML Tags:** `<html>`, `<head>`, `<body>`, `<div>`, `<span>`, etc.
- **Attributes:** `id`, `class`, `href`, `src`, etc.
- **DOM Structure:** The hierarchical organization of elements.

#### Common HTML Tags and Their Uses:

- **Headings:** `<h1>`, `<h2>`, `<h3>`, etc.
- **Paragraphs:** `<p>`
- **Links:** `<a href="URL">Link Text</a>`
- **Images:** `<img src="image.jpg" alt="description">`
- **Lists:** `<ul>`, `<ol>`, `<li>`
- **Tables:** `<table>`, `<tr>`, `<td>`

#### Basics of CSS:

- **Selectors:** Element selectors, class selectors, ID selectors.
- **Styling:** Applying styles using CSS.
  ```html
  <style>
    .class-selector {
      color: blue;
    }
    #id-selector {
      font-size: 20px;
    }
  </style>

```
## 3.Fetching Web Pages with Requests

#### Introduction to the requests Library:

* **Requests:** Sending HTTP requests to fetch web content.
```python      
pip install requests
```
#### Sending GET Requests and Handling Responses:

```python
import requests
url = "http://google.com"
response = requests.get(url)
```

### Handling HTTP Responses:

#### Status Codes:
 
    200: OK
    300: Redirection
    400: Client Error (e.g., 404 Not Found)
    500: Server Error (e.g., 500 Internal Server Error)
## 4.Parsing HTML with Beautiful Soup

### Learning Objectives:

- Parse HTML documents using Beautiful Soup.
- Extract specific elements and data from web pages.

### Introduction to Beautiful Soup

Beautiful Soup is a Python library named after a Lewis Carroll poem of the same name in "Alice's Adventures in Wonderland". Beautiful Soup parses unwanted data and helps organize and format messy web data by fixing bad HTML and presenting it in easily-traversable XML structures. In short, Beautiful Soup is a Python package that allows us to pull data out of HTML and XML documents.

### Installing Beautiful Soup:

```bash
pip install beautifulsoup4
```

### Commonly Used Methods and Attributes:

    soup.title: The <title> tag of the HTML document.
    soup.body: The <body> tag of the HTML document.
    soup.find(): Finds the first instance of an element.
    soup.find_all(): Finds all instances of an element.

        
