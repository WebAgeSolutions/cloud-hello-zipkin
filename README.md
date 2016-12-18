# cloud-hello-zipkin

This is a sample application in Spring Cloud.  It hosts a single 
resource, '/hello-message?name=<string>'.  It answers back 'hi there'.

It can be configured to fail, throwing exceptions after it receives some number of calls.  It will then reset when left idle for 30 seconds or more.
This behavior is useful for trying out the Hystrix circuit-breaker package.

# Configuration:

Set the following options as per Spring Boot's conventions.

server.port The port the server starts up on.  
failAfter.enabled Set true to turn on the simulated failures.  
failAfter.count How many requests to fail after?  
serverId A server identification that is returned in the message.


