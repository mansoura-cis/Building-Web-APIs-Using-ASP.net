# Building-Web-APIs-Using-ASP.net
Learning APIS
# What is Web API?
  ## What is the Web?

- Nowadays, networking and the Internet are very popular. Software running on different computers can "talk" to each other. The "languages" used by software to "talk" are protocols. You may have heard about protocols such as TCP, HTTP, FTP, etc.

- The Web is a group of computers in a network, and they communicate with each other through HTTP protocol, typically. The Web can be big or small, for example:

   - On an intranet of a company, if there are some computers that communicate with each other through HTTP and share documents via a web browser, that can be considered a SMALL web.
   - On the Internet, billions of computers and devices communicate through HTTP, forming a BIG web. As a matter of fact, it is one of the largest things on the Earth - the World Wide Web.
## What is a Web Server
- Usually, when software is communicating across a network, the role of each software application may be different. If an application holds the resources, such as data or program logic, and can provide these resources to other applications, we refer to the application, and the computer, as a server. In contrast, if the application does not have the resources it needs, it has to request the resources from other applications through the network. We call this role a client.

If an application can provide data and/or computing power across a web, we call it a web server. Because the computers/devices on a web are connected by HTTP protocol, we can easily infer that a web server must provide/expose resources through HTTP protocol.

There are a variety of resources the web server can provide to the web clients, but we can categorize resources into just two categories - data and computing power. Data can be represented by many things on the server, such as an HTML page, a PNG image, an MP3/MP4 file or a bunch of records in a database. Computing power means the computing ability of a server. Servers can typically offer greater computing resources than a client may possess, depending on the computer hardware used.

The client can send parameters to the server through requests. After the server accepts the parameters and executes a computation of some sort, it returns the result back to the client through a response.

If a web server provides data resources, and the data are in HTML format (we know a browser can render HTML content), we call this web server resource a Website.
If a web server provides a data resource, and the data is serialized in XML, JSON or other formats, we call this a Data Web Service or Data Service.
If a web server provides computing power resources, which means the web client can invoke the computing power on the web server remotely, and the web server will respond with the computing result (in proper format), we call this web server Web Services or Web API

> As you may notice, regardless of the type of resources, there must be some result or data in the response to the client. The result data proves the existence of resources on the server, and we call these data the representation of resources.

## What is Web API
API stands for Application Programming Interface. An API is critical for referencing and invoking members in class libraries. If you want to use the members in class libraries successfully, your code must comply with the API defined by the developer of those class libraries.

After referencing a class library, the application can easily call or utilize the functionality of the class library on a single computer. The real problem is when the application and class library are not on the same computer. How do we make a call to an API on a different computer than our client?

There are several generations of solutions for this problem, such as Remote Procedure Call (RPC), Common Object Request Broker Architecture (CORBA), etc. Eventually, developers grafted remote calls onto web servers. This results in the class libraries residing on the web server and exposing the API of class libraries through the HTTP protocol.

In this way, web servers centralize the computing power and publish it as web services, while the web clients consume the computing power remotely. Since the web clients are still calling the API of the class libraries but remotely through the web, we call this kind of web service, Web API. In short, if a web service acts as the wrapper of class libraries and just exposes remote computing ability, we call it Web API.

There are many styles and rules for designing these web APIs,

Simple Object Access Protocol (SOAP) provides a convention for representing remote procedure calls and responses. If a web service adopts SOAP, we call this web service a SOAP Web Service or SOAP Web API.
Representational state transfer (REST) is a set of architectural constraints (NOT a protocol or standard), for web application design. Since a web service is a kind of web application, we can apply REST constraints to the design of web services. Once a web service adopts REST concepts, we call it a RESTful Web Service or RESTful Web API.
In much the same way that we simply call a local variable, "variable", and call a parameter variable, "parameter", we always simplify the name SOAP Web Service to Web Service, and the RESTful Web Service to Web API. This implies that most of the modern Web APIs tend to adopt the REST concept as their design principle.

So, what is REST? In the next module, we will give it a closer look.
