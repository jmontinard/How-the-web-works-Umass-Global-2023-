# How-the-web-works-Umass-Global-2023-
How the web works Umass Global 2023 - jmontinard
1- What is HTTP? // HTTP is Hypertext transfer protocol HTTP is a protocol for fetching resources such as HTML documents. It is the foundation of any data exchange on the Web and it is a client-server protocol, which means requests are initiated by the recipient, usually the Web browser.

2- What is a URL? Uniform Resource Locator - A URL is nothing more than the address of a given unique resource on the Web. In theory, each valid URL points to a unique resource. Such resources can be an HTML page, a CSS document, an image, etc.

3- What is DNS? -The Domain Name System (DNS) is the phonebook of the Internet. Humans access information online through domain names, like nytimes.com or espn.com. Web browsers interact through Internet Protocol (IP) addresses. DNS translates domain names to IP addresses so browsers can load Internet resources.

4- What is a query string? - A query string is the portion of a URL where data is passed to a web application and/or back-end database. The reason we need query strings is that the HTTP protocol is stateless by design. (for example, www.techopedia.com/somefile.html), and the query string is whatever follows the question mark sign (“?”).
5- What are two HTTP verbs and how are they different? - HTTPS is encrypted and secured using digital certificates, while HTML is not. When you visit a website using HTTPS, your connection to that site is encrypted.
6- What is an HTTP request? -An HTTP request is made by a client, to a named host, which is located on a server.
7- What is an HTTP response? -An HTTP response is made by a server to a client. The aim of the response is to provide the client with the resource it requested, or inform the client that the action it requested has been carried out; or else to inform the client that an error occurred in processing its request.
8- What is an HTTP header? Give a couple examples of request and response headers you have seen. - An HTTP header is a field of an HTTP request or response that passes additional context and metadata about the request or response.
Headers provide additional information about the request or the response. Here are some examples:
Request
headers: Host, User-Agent, Accept, Cookie, Cache-Control
Response headers: Content-Type, Last-Modified, Set-Cookie, Cache-Control

9- What are the processes that happen when you type “http://somesite.com/some/page.html” into a browser?

Step 1: IP Address Lookup - The first thing that needs to happen is your browser needs to get the IP address of the server hosting the web resource you’re trying to access. Giving your browser a URL or a domain name doesn’t actually give it enough information to know where to reach a web server.
Step 2: Initial connection to the server - Once your browser knows where the web server is, it can establish a connection to it. The first layer of connection it needs to establish uses a protocol called Transmission Control Protocol, or TCP This is one of the basic protocols on the internet.
Step 3: Connect using HTTP - You might have been confused in the last section when we talked about using the TCP protocol to connect to a server because we just said up where we were talking about the parts of the URL that “HTTP” is the protocol. That’s because TCP is the internet protocol used to connect two computers over the internet while HTTP is a web protocol used to exchange web data.
Step 4: Connecting with HTTPS (i.e. HTTP using TLS/SSL) - That’s where HTTPS comes in. HTTPS adds another protocol to the mix—TLS, or as it’s often better known, SSL—which is a process that can be used to make all the data sent and received between a web server and a web browser secret to everyone except them. TLS/SSL does this by encrypting the data, which means encoding the data using a secret cipher.
Step 5: Web content is received - Finally, once the TCP connection, HTTP connection, and HTTPS connection are all established, your browser will receive the data from the web server located at the address you entered. If that’s a webpage, that data will be in HTML (hypertext markup language) format, a data format specific to the web.

p2 ?

Part Two: Practice Tools
Using curl, make a GET request to the icanhazdadjoke.com API to find all jokes involving the word “pirate”
https://icanhazdadjoke.com/search?term=pirate

Use dig to find what the IP address is for icanhazdadjoke.com

dig https://icanhazdadjoke.com
Make a simple web page and serve it using python3 -m http.server. Visit the page in a browser.
