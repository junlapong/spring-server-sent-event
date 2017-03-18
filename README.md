# Sending events from Server using Spring
[Server Sent Events](https://www.w3.org/TR/eventsource/) is a mechanism of pushing data to client over HTTP or by using [push server protocols](https://en.wikipedia.org/wiki/Push_technology). It is standardized as part of HTML5 by W3C.

Spring Web MVC framework has a class named [SseEmitter](http://docs.spring.io/spring/docs/current/javadoc-api/org/springframework/web/servlet/mvc/method/annotation/SseEmitter.html) which allows server to send out stream of data gradually (i.e. in chunks) after the client has invoked an endpoint and established a connection. It can be used to continously send message updates or continous data streams to clients for having enhanced user experience.

This is demonstrated as a POC in 2 ways -




Sample app explaining how server can send events periodically to client for single endpoint invocation via normal mode and reactive mode (i.e. using Spring 5.0)
