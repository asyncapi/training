# Video 4: AsyncAPI and OpenAPI

Hello again! Welcome to a new video about AsyncAPI. This video will discuss what AsyncAPI and OpenAPI have in common and how they differ. 

Ready or not, here we go! 

## What is OpenAPI?

OpenAPI is a standard for describing application programming interfaces (APIs). This specification defines an open, vendor-independent description format for API services. In particular, OpenAPI can describe, develop, test, and document REST-compliant APIs.

The current OpenAPI specification grew out of the predecessor project, Swagger. The development company SmartBear subjected the existing Swagger specification to an open license, handing over both maintenance and development of the initiative to the Linux Foundation. In addition to SmartBear, members of the OpenAPI initiative include industry giants such as Google, IBM, and Microsoft.

## Similarities between AsyncAPI and OpenAPI

AsyncAPI's ultimate goal is to work with EDA architectures as simply as with Rest APIs. The AsyncAPI specification in the asynchronous world is analogous to OpenAPI in the synchronous world. 

Both initiatives share numerous similarities:

- Contract-first philosophy
- Agnostic implementation
- Similar syntax
- A tooling ecosystem 
- Extensible by including new properties with the prefix x-
- They protect information consumption using different security schemes. (Example: user and password, API keys, certificates, OAuth, OIDC, etc.)


## Differences between them

 As we have seen, the two initiatives are significantly similar, but they also cover significantly different fields. REST APIs have a specific function that requires their methods and documentation approaches. REST APIs have, among others, a great solution in the form of OpenAPI, a set of standardized documentation methods for enabling tools and interactivity.
 
 On the other hand, message-based APIs are different because they require solutions for the caveats and intrinsic considerations of message-based architectures. AsyncAPI's tagline says it best: "REST APIs have OpenAPI. Messaging has AsyncAPI."
 
 It's essential to understand that while the two solutions have a lot in common, they are also wildly divergent. Both OpenAPI and AsyncAPI allow for more significant cooperation and collaboration between different documented APIs. Still, OpenAPI is a solution for REST, and AsyncAPI is a solution for message-based architectures. Each aims to serve a different domain.

## AsyncAPI and OpenAPI comparison

As you can see, you'll find lots of similarities between OpenAPI and AsyncAPI!

![](https://user-images.githubusercontent.com/19964402/161353808-430cb73e-e2a3-4913-ad5e-6cccdeeaa997.png)

In event-driven architectures, you have more than one protocol, and therefore, some things are different. Let's check out the following comparison chart, inspired by [Darrel Miller's blog post](https://www.openapis.org/news/blogs/2016/10/tdc-structural-improvements-explaining-30-spec-part-2):

![](https://user-images.githubusercontent.com/19964402/161353528-23fd7a02-7917-4e1b-856d-c66b8456f373.png)

 ## Goodbye to the viewer
 
Thank you for joining us in today's adventure! I hope today's content helped you clarify your doubts. Join us in the next video to learn about AsyncAPI and its environment!
