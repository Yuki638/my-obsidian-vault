### HTTP Protocol

The HTTP protocol can be thought of as a general protocol of transferring information through the web.

This includes many types of [[REST API]]. [[REST API]] function by sending a request and the request is communicated via HTTP message. The HTTP message usually contains a [[JSON]] file.

When you, the client uses a web page your [[browser]] sends an [[HTTP request]] to the [[server]] where the page is hosted. The [[server]] tries to find the desired resource by default "index.html".

If your request is successful, the [[server]] will send the object to the client in an HTTP response; this include information like the type of the resource, the length of the resource, and other information.

| Resources  |
| :--------: |
| Index.html |
| Image.png  |
|  File.txt  |
when the request is made for the information , the [[web server]]s sends the requested information, that is, one of the files. 



### Uniform Resource Locator:URL

A [[URL]] is the most popular way to find resources on the web.

#### Overview of HTTP

* **Scheme:** [http://](#)
* **Internet address or Base [[URL]]:** used to find the location, for example:[www.ibm.com](https://www.ibm.com) and [www.gitlab.com](https://gitlab.com)
* **Route:** location on the web [[browser]], for example: 
  [/images/IDSN logo.png](#) 

[http://www.ibm.com/images/IDSN logo.png](http://www.ibm.com/images/IDSN logo.png) 


### Request Message


| Request start line |                          /Get/index.html<br>    HTTP/I.O                          |
| :----------------: | :-------------------------------------------------------------------------------: |
|   Request Header   | user-Agent: python-<br>requests/2.2.4.0<br>Accept-Encoding:<br>     gzip,deflate: |


### Response Message


| Response Start Line |                           HTTP/1.0 200 OK                           |
| :-----------------: | :-----------------------------------------------------------------: |
|   Response Header   |                server: Apache-cache <br>UNCACHEABLE                 |
|    Response Body    | ```<!Doctype html><html><body><h1> heading</h1></body</html><br>``` |


### Status Code


| 1xx |      Infornational      |
| :-: | :---------------------: |
| 100 | Everything so far is Ok |
| 2xx |         Success         |
| 200 |           Ok            |
| 3xx |       Redirection       |
| 300 |    Multiple Choices     |
| 4xx |      Client Error       |
| 401 |      unauthorized       |
| 403 |        Forbidden        |
| 404 |        Not Found        |
| 500 |      Server Error       |
| 501 |     Not Implemented     |


### HTTP Methods


| **HTTP Methods** |           **Description**           |
| :--------------: | :---------------------------------: |
|     **GET**      | Retrieves data from the [[server]]. |
|     **POST**     |     Submits data to [[server]].     |
|     **PUT**      | Updates data already on [[server]]. |
|    **DELETE**    |    Deletes data from [[server]].    |

## Requests modules in python 

Requests is a python [[library]] that allows you to send [HTTP/1.1](#) requests easily. We can import the [[Library]] as follows:

```python
import requests

url='https://www.ibm.com/'
r = requests.get(url)
r.status_code
r.request.headers
r.request.body
header = r.header
header['date'] #obtaining the date the request was sent
header['content type'] #indicates the type of data
r.encoding
r.text[0:100]
```

### Get Requests with URL 

You can use the GET method to modify the results of your [[Query]]. For example , retrieving data from an [[API]].

### GET Request


| **Base URL**                            | **Route**                        |
| --------------------------------------- | -------------------------------- |
| <font color = "blue">httpbin.org</font> | <font color = "blue">/get</font> |

| <font color = "blue">httpbin.org/get</font> |
| ------------------------------------------- |

We send a GET request to the [[server]]. We have the Base [[URL]] in the Route.

### Query String


| **Start of [[Query]]** | **Parameter Name** |     | **Value** |     | **Parameter Name** |     | **Value** |
| :--------------------: | :----------------: | :-: | :-------: | :-: | :----------------: | :-: | --------- |
|           ?            |        name        |  =  |  Joseph   |  &  |         ID         |  =  | 123       |

After GET is requested we have the [[Query]] string.This is a part of a Uniform Resource Locator ([[URL]]) and this sends other information to the [[web server]].

The start of the [[Query]] is a "?" followed by a series of parameter and value pairs.

The first parameter name is "name" and the value is "Joseph".
The second parameter name is "ID" and the value is "123".

Each pair, parameter, and value is separated by an equal sign "=". The series of pairs is separated by the ampersand "&".

### Create Query String

```python
url_get = 'http://httpbin.org/get'
```

We have the base [[URL]] with GET appended to the end.

```python
payload = {"name":"Joseph", "ID":"123"}
r = requests.get(url_get,params = payload)
```

To create a [[Query]] string , we use the dictionary payload. The keys are the parameter names, and the values are the value of [[Query]] String. Then we pass the dictionary payload to the params parameter of the **get()** function.
```python
r.url
r.request_body
r.text
```

We can view the response as text

```python
r.headers['Content type']
```

we can look at the key 'Content Type' to look at the content type.

As the content 'Content-Type' is in the [[JSON]], we format it using the method json(). It returns a python Dict

```python
r.json()
```

### POST Requests

Like a GET request, a POST request is used to send data to a [[server]], `but the POST request sends the data in a request body, not the [[URL]].

In order to send the POST request in the URL, We change the route to POST. This endpoint will expect data and its a convenient way to configure a **HTTP** request to send Data to a [[server]].

```python
url_post = "http://httpbin.org/post"
```

```python
payload = {"name":"JOseph","ID":"123"}
r_post = requests.post(url_post, data=payload)
```

### Compare POST and GET Requests

```python
print("POST request URL",r_post.url)
print("GET request URL",r.url)
```

<font color= "red">POST request URL : </font>https://httpbin.org/post
<font color= "red">GET request URL : </font> http://httpbin.org/get?name=Joseph&ID=123

We see POST request has no name or value pair in its [[URL]].

If we compare the POST and GET request body. We see only the POST request has a body and we can view the key performance to get the payload.