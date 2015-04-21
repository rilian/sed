#### Metaprogramming
> Metaprogramming is the writing of computer programs with the ability to treat programs as their data. It means that a program could be designed to read, generate, analyse and/or transform other programs, and even modify itself while running.
* example..
--------------

#### REST
> Representational state transfer;
* example..
--------------

#### SOAP
> Simple object access protocol;
* example..
--------------

#### SOLID
> * S: A class should have only one reason to change.
> * O: Software entities (classes, modules, functions, etc.) should be open for extension, but closed for modification.
> * L: Child classes should never break the parent class' type definitions.
> * I:
> * D: High-level modules should not depend on low-level modules. Both should depend on abstractions.
     Abstractions should not depend upon details. Details should depend upon abstractions.

#### Service oriented architecture
> Service-oriented architecture (SOA) is an evolution of distributed computing based on the request/reply design paradigm for synchronous and asynchronous applications.
* example..
--------------


Basic
HTTP
HTTP functions as a request-response protocol in the client-server computing model. A web browser, for example, may be the client and an application running on a computer hosting a web site may be the server. The client submits an HTTP request message to the server. The server, which provides resources such as HTML files and other content, or performs other functions on behalf of the client, returns a response message to the client. The response contains completion status information about the request and may also contain requested content in its message body.

A web browser is an example of a user agent (UA). Other types of user agent include the indexing software used by search providers (web crawlers), voice browsers, mobile apps, and other software that accesses, consumes, or displays web content.

HTTP is designed to permit intermediate network elements to improve or enable communications between clients and servers. High-traffic websites often benefit from web cache servers that deliver content on behalf of upstream servers to improve response time. Web browsers cache previously accessed web resources and reuse them when possible to reduce network traffic. HTTP proxy servers at private network boundaries can facilitate communication for clients without a globally routable address, by relaying messages with external servers.

HTTP is an application layer protocol designed within the framework of the Internet Protocol Suite. Its definition presumes an underlying and reliable transport layer protocol, and Transmission Control Protocol (TCP) is commonly used. However HTTP can use unreliable protocols such as the User Datagram Protocol (UDP), for example in Simple Service Discovery Protocol (SSDP).

HTTP resources are identified and located on the network by Uniform Resource Identifiers (URIs)—or, more specifically, Uniform Resource Locators (URLs)—using the http or https URI schemes. URIs and hyperlinks in Hypertext Markup Language (HTML) documents form webs of inter-linked hypertext documents.

HTTP/1.1 is a revision of the original HTTP (HTTP/1.0). In HTTP/1.0 a separate connection to the same server is made for every resource request. HTTP/1.1 can reuse a connection multiple times to download images, scripts, stylesheets, etc after the page has been delivered. HTTP/1.1 communications therefore experience less latency as the establishment of TCP connections presents considerable overhead.

TCP/IP

SPDY

Patterns
Convention over Configuration in Active Record
When writing applications using other programming languages or frameworks, it may be necessary to write a lot of configuration code. This is particularly true for ORM frameworks in general. However, if you follow the conventions adopted by Rails, you'll need to write very little configuration (in some case no configuration at all) when creating Active Record models. The idea is that if you configure your applications in the very same way most of the time then this should be the default way. Thus, explicit configuration would be needed only in those cases where you can't follow the standard convention.



Other
Metaprogramming

Multitenancy
У многопоточных приложений в одном процессе одновременно может выполнятся несколько потоков (нитей). Например, веб-сервер может обрабатывать несколько запросов одновременно.

У стандартного интерпретатора Ruby (MRI) потоки не могут выполняться параллельно. Т.е. у приложения может быть несколько потоков, но работать одновременно будет только один. Это известная проблема. В некоторых альтернативных интерпретаторах этой проблемы нет.

И что бы один сервер мог обрабатывать несколько потоков одновременно, запускают параллельно несколько экземпляров приложения. Для распределения запросов между экземплярами приложений обычно используют фронтенд сервер (обычно nginx).


http://www.slideshare.net/tardate/multitenancy-with-rails

Dispatch: https://hackpad.com/ep/pad/static/9nJ4XusVtmv
DataXu:   https://hackpad.com/ep/pad/static/7azeb2PQlw8
