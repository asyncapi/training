# Video 4: AsyncAPI and OpenAPI

Hello again! Welcome to a new video about AsyncAPI, the open source initiative that seeks to improve the current state of Event Driven Architectures (EDA). If you wanna know more about the spec just check the previous video (3) on "What is AsyncAPI". This video will discuss what AsyncAPI and OpenAPI have in common and how they differ. 

Ready or not, here we go! 

## What is OpenAPI

OpenAPI is a standard for describing application programming interfaces (APIs). This specification defines an open, vendor-independent description format for API services. In particular, OpenAPI can describe, develop, test, and document REST-compliant APIs. Understood as a software architecture for hypermedia systems on the World Wide Web, REST often uses the HTTP protocol.

The current OpenAPI specification grew out of the predecessor project, Swagger. The development company SmartBear subjected the existing Swagger specification to an open license, handing over both maintenance and development of the initiative to the Linux Foundation. In addition to SmartBear, members of the OpenAPI initiative include industry giants such as Google, IBM, and Microsoft.

## Similarities between AsyncAPI and OpenAPI

AsyncAPI's ultimate goal is to work with EDA architectures as simply as with Rest APIs. For those who don't know what REST APIs are, we will briefly say that interface between systems and that uses HTTP to obtain data or generate operations on that data in all possible formats.

Back to the comparison, the AsyncAPI specification in the asynchronous world is analogous to OpenAPI in the synchronous world. 

Both initiatives share numerous similarities:

- Contract-first philosophy, also known as API-first. In other words, design API first and then implement it.
- Implementation-agnostic, it refers that is compatible with various systems. 
- Similar syntax
- A tooling ecosystem 
- Extensible
- They protect information consumption using different security schemes. (Example: user and password, API keys, certificates, OAuth, OIDC, etc.)

## Differences between AsyncAPI and OpenAPI

As we have seen, the two initiatives are significantly similar, but they also cover significantly different fields. 
 
OpenAPI is a solution for REST, and AsyncAPI is a solution for message-based architectures. Each aims to serve a different domain. We could say that the big difference between the two is that OpenAPI, which focuses on synchronous communication, is used for HTTP protocol. AsyncAPI is used for multiple different protocols designed for async communication.

These are two complete different architectures that require different specifications. That is the main difference between OpenAPI and AsyncAPI. But, yeah, let's jump into details.

## AsyncAPI and OpenAPI comparison

Microservices architecture makes something pretty cool: to split up huge globs of code into tiny, manageable pieces. That’s the way different teams can work on pieces simultaneously, sharing the fun!

Making different combinations of microservices appears them as the most efficient way of creating something new. Making combinations as a puzzle. REST calls were the main method to stick those pieces together, acting as glue.

Jesse Menning makes it very clear in this fantastic [article](https://www.asyncapi.com/blog/openapi-vs-asyncapi-burning-questions) that we highly recommend.

That method worked pretty well in synchronous communication, but it has its limitations. People eventually realized that REST wasn’t always the best tool for laying the game. The search for a new kind of glue starts as a way of facilitating asynchronous communication.

The internet of things acted as a real game-changer. Since it was introduced, everything seems to be connected to the Internet. And everything Is everything, including vacuum cleaners, heaters, ovens, cars... That is amazing but not that easy. Every gadget doesn’t always have solid internet connections. Asynchronous communication rises as a better way to connect them.

Establishing asynchronous communication between microservices makes them more reliable, faster, easier to scale, and more agile to adopt.

![Protocols supported](https://user-images.githubusercontent.com/77982319/165746023-ed78afbc-598b-4401-843e-6ac851d30303.jpg)

AsyncAPI and OpenAPI are now both under the umbrella of the Linux Foundation. That beautiful coincidence facilitates its combined used, opening a world of API possibilities that can be explored and covered. 

Being hosted by Linux Foundation, it is possible to say that AsyncAPI and OpenAPI share a wide common ground, well supported and stable. They share open standards with community governance. They should also continue to be integrated with open-source tooling and commercial products.

Both are heading straight to a promising future, wide open.

 ## Goodbye to the viewer
 
Thank you for joining us in today's adventure! I hope today's content helped you clarify your doubts. Join us in the next video to learn about AsyncAPI and its ecosystem!