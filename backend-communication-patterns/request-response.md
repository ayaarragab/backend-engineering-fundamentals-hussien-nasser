# Request-response model

## Here's my notes from Hussien Nasser's course "Backend Engineering Fundamentals" in its second section, first video

### Nature

+ It's a Simple, elegant model. Where you have a tcp connection per request, connection closes when client recieves the response unless keep-alive header is set to true.

+ It's the base for the other models, which had higher complexity, and handled cases which request/response couldn't handle.
---
+ Some cases where Request/Response is the best option to use:
  + Simple, fast operations (CRUD APIs)
  + Well-supported by all HTTP clients and servers
  + Fits RESTful design perfectly
---
+ Some cases where it's not the best option to use:
  + Real-time
  + Long-running requests
  + When you have complex workflow (a service that sends msg to another one and another one sends it to another)

**Aya Ragab**

