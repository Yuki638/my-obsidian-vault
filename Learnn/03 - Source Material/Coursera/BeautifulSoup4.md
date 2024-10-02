```python
import requests
from bs4 import BeautifulSoup

url = 'www.google.com'
r = requests.get(url)
soup = (r.text,'html.parser')
print(soup.prettify()) #basically makes the html code prettier like in a formatted order
```

links: [[web scraping]] 
### Why did we use 'html.parser' ?

so the ``` r.text``` is just a bunch of strings that we got through the requests [[module]] and the computer doesn't know it's a html string. so to make our  python code understand that its HTML and not any other string we use <font color ="lightgreen">'html.parser'</font>.

<font color ="red">In the words of ChatGPT</font> --> 
```
When you visit a website, the webpage is written in a language called **HTML** (HyperText Markup Language). HTML is like the blueprint for the webpage — it tells the browser how to display the page (where to put the text, images, links, etc.).

Now, when you use `requests` to get a webpage, what you get back is just a long string of HTML. But the computer doesn’t automatically understand that this is HTML. It’s just a bunch of text.

So, to **help Python understand** that the text we got from the website is actually HTML and not just random text, we use `BeautifulSoup` and tell it, "Hey, treat this text like HTML!" That's where `'html.parser'` comes in.

Why Do We Need 'html.parser'?

  HTML is special: It's not just regular text; it has a specific structure with tags (`<html>`, `<body>`, `<h1>`, etc.).
  
  Parsing HTML: The `'html.parser'` helps `BeautifulSoup` break down the HTML and understand its structure so that you can easily grab things like the title, links, or paragraphs.

Here’s an analogy:

  Imagine you have a recipe written in code language, and you want to turn it into a regular recipe you can read.

     response.text gives you the recipe, but it’s still in code.
     
     html.parser is like a tool that reads that recipe code and turns it into something understandable and readable.
```
