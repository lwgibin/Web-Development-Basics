# Web-Development-Basics

```
Information extracted from Le Wagon's free online introduction course.
```

## Web 101
### What’s the Web compared to the Internet?
How can we differentiate the Web and the Internet?

The Internet is the infrastructure that connects computers on a worldwide network. You can see it as the wires and cables that carry the information around the world.

The Web is included in the Internet. The Web is everything that passes through the Internet, via the HTTP protocol.

### WTF is HTTP?
HTTP stands for Hyper Text Transfer Protocol.
It is a protocol to transfer resources (== files) between two machines (~ computers).

This protocol relies on a very simple system:
- The machine from which you want to access a web page is called the client
- The machine which hosts the content of the website is called the server
- The client sends an HTTP request to the server, with the url of the page to open
- The server processes this request, and sends back an HTTP response to the client, with the content of the page
- The client processes this response, and displays the web page

### Interacting with a website
The most important takeaway of this chapter is the following:

Any action on a website triggers an HTTP request.

Wether you type a url in the address bar, click on a link or submit a form, it will trigger an HTTP request sent by the client to the server.

### Static vs Dynamic
If the content asked in the HTTP request is static, the server will basically read corresponding HTML file’s content from its hard drive and send it back to the client via the HTTP response.

If the content is dynamic, for instance if the HTML file’s content is different for two different connected users (as in two Facebook profile pages), it won’t be as simple.
The server needs to be more intelligent. It needs to “speak” a back-end programming language. At Le Wagon, we’ll use Ruby, but this back-end programming language could be php, Python, Java, etc…
In that case, the HTTP request is processed by the back-end code, this code will probably query a database and finally build the HTML file with the right content.
Then it will send the HTML file back to the client via the HTTP response.

In both cases, it all comes down to this cycle:
<img width="749" alt="client_server_cycle" src="https://user-images.githubusercontent.com/25816956/27743051-093d752e-5dbb-11e7-8531-c299a068242c.png">

### Main takeaways
- The web relies on two machines communicating
- The client is the machine requesting some content
- The server is the machine hosting the website (~ data + code)
- They both communicate via the HTTP protocol
- The HTTP protocol consists in transfering files
- This transfer relies on a system of request / response
- The client sends a request to the server
- The server processes the request and builds the response with an HTML file
- The client receives the response and processes the HTML file to display the web page in a browser
