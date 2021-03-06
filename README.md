# SpringBoot-Async

## For scaling heavy system, Java provides a mechanism for executing expensive job in background with Java Thread Pool and Future to manage final Result. 

## Spring Framework makes more easy with annotation <i>@Async</i>. 

## Requirements to Run the Application:
1. Java
2. Maven
3. IDE of your choice

## The @Async Annotation
By making a Servlet asynchronous, we can return the thread calling the Servlet to the container and continue the remainder of the request on another thread. 
      (*from Oracle) In modern web applications there are times when you need to asynchronously handle some part of the request, so that the web container can continue serving other requests in a seamless fashion. One example is a chat room application. In this type of application you want to enable long-lived client connections with a servlet. You don't want a server thread to be blocked for a long period of time serving a request from a single client. You want the servlet to process a request from the client and then free up the server thread as quickly as possible for other work. In other words, you want the request to be processed and a response generated asynchronously. 

## Rest API 
Multiple HTTP endpoints exposed as an API to external world on which you continuously receive event. 

## Brackground
When you annotate something in Spring (ex. @Async) what you are actually doing is telling Spring “when you load this class, you should apply AOP as methods are invoked” (i.e. points that Spring will invoke prior/after to invoking the function itself).
