# Push vs Poll models

## Here's my notes from Hussien Nasser's course "Backend Engineering Fundamentals" in its second section, 4rd, 5th, 6h videos

### Quick Intro

In any type of application—whether websites, mobile apps, or others—we typically have a sender, a receiver, and one or more connections established between them. Different backend communication models define how data is transferred between the sender and the receiver, and how these connections are managed. By choosing and tuning these models, we aim to achieve the highest performance, the lowest cost, and the most efficient use of resources.

### Push model

+ In basic request/response model, client sends a request to the server whenever it needs data from it, a connection is established, then server responds with the appropriate response.
+ There's a difference here, client sends a request, a connection is established, then server  proactively pushes data to the client whenever new data is available, without the client having to request it again.
**Pros and Cons**
+ Good for Realtime.
+ Some of its limitations is that client must be online and might not be able to handle the stream of data coming from the server.

### Poll model

+ When client sends a request to the server, server immediately replies with a handler (i.e., job id).
+ If it’s short polling, the client sends a request every few seconds (or a fixed interval) to ask: “Is my job ready?”
+ If it’s long polling, the client sends a request, and the server keeps the request open until the job is complete or a timeout occurs.
+ Once the job is done, the server responds with the result, and the client can stop polling or start a new request if needed.
**Pros and Cons**
+ Good for long-running requests.
+ Less efficient for realtime updates compared to push-based models.

### Thank you


