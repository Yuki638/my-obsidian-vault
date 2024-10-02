```python
import requests
r = requests.get('https://dev.to/jfmartinz/hacktoberfest-2024-everything-you-need-to-know-29h7')
print(r.text) #just going to display rough html text
print(r.status_code) #status code for the website visiting i.e. 200 if okay
print(r.headers) #display the headers
print(r.encoding) #displays the encoding
```

the above snippet explains how GET works with the help of requests [[module]] in python so that we can do [[web scraping]] efficiently 
first we use the `requests.get` to get the HTML of the URL we provided in this case [link](https://dev.to/jfmartinz/hacktoberfest-2024-everything-you-need-to-know-29h7) (FAQ in Hacktober Fest). 


### <font color ="Teal">What exactly is requests module???</font>

Imagine the web is like a giant library. Each webpage is like a book in that library. The requests [[module]] is like a friendly librarian who helps you go to the library and ask for a specific book

### <font color ="teal">GET request</font>

So lets take the above example GET request is like when the librarian gets the book for you that you ask. GET request gives you the webpage contents and display it as HTML text or JSON.

### <font color ="teal">POST request</font>

