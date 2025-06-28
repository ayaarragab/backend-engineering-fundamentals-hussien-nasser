# Syncronous Vs Asyncronous

## Here's my notes from Hussien Nasser's course "Backend Engineering Fundamentals" in its second section, 2nd video
---

### Quick note before reading this 

+ I'm focusing on making things make sense to whoever read these notes, as when I was studying I focused on this aspect too much, and because this course is mainly for SW engineers who had work experience in backend, it was a little bit hard to understand some concepts from the first moment, but the effort I did to understand paid off :)

### What does really asyncronous and syncronous mean?

#### Here's a ChatGPT analogy that helped me ALOT

+ Synchronous Analogy:
It’s like going to a repair shop to fix something.
You go there, sit down, and wait right there until they finish fixing it.
You don’t leave or do anything else—you just stay until it’s done.

In other words:
You wait until the job is complete before moving on.

+ Asynchronous Analogy:
It’s like going to the repair shop, dropping off your item, and then leaving to do other errands.
When they finish, they call you to come pick it up.
You didn’t have to sit and wait—you continued with your tasks until you got notified.

In other words:
You send the request, go do other things, and later get notified when the job is ready.

#### What does that mean in backend processing

+ Remember we're only talking about `Backend` now, the style of processing that is done within your backend app, let's take an example for a syncronous backend app: