### Outline
* What is [[API]].
* [[API]] Libraries.
* [[REST API]]
    * Request and Response.
# <u>What is API ?</u>

"[[API]] lets two pieces of software talk to each other."
You can use [[API]] to communicate with other software via inputs and outputs.

e.g- **[[Pandas]]** We use the pandas [[API]] to process the data by communicating with the other [[software component]].
![[screenshot_04092024_232712.jpg]]

# <u>REST APIs</u>

[[REST API]] allows you to communicate through the internet allowing you to take advantage of resources like storage , access more data , AI algorithms ,and much more. 

<font color="red">RE</font>presentational 
<font color="red">S</font>tate
<font color="red">T</font>ransfer APIs

* [[REST API]] helps to interact with web services, that is applications that you call through the internet.
* they have set of rules:
	    1.Communication
	    2. Input or Request
	    3. Output or Response
---
You or your code can be thought as a client 
the [[Web Service]] is referred to as a resource. The client sends requests to the resource and the response to the client

#### <u>HTTP Method</u>

A way of transmitting data over the internet. We tell the [[REST API]] what to do by sending a request.
The request is usually communicated via an HTTP message. The HTTP message usually contains JSON file. This contain instruction for what operation we would like the service to perform. This Operation is transmitted via the internet.
![[Screenshot 2024-09-05 at 00-37-56 Application Program Interface Coursera.png]]

The service performs the operation in a similar manner, the [[Web Service]] returns a response via an HTTP message , Where the information is usually returned via a JSON file. This information is transmitted back to the client.
![[Screenshot 2024-09-05 at 00-43-55 Application Program Interface Coursera.png]]
