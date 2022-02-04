
## Video 2: What kinds of API architectures exist

- Web Architecture definition
- Monolithic architecture
- Microservices architecture
- Layered or N-tier
- Service-oriented architecture
- Event-driven architecture
- EDA and AsyncAPI

Hello everyone! Welcome!

In this video, we're going to talk about the different types of API architectures that exist. We'll try to explain their meaning, discover what they bring, what they're used for, and how to analyze them. 

Let's start with web architectures!

## Web Architecture definition 

Web architecture is the way in which the pages of a website are structured and linked together in a logical and coherent manner. It could be said to refer to the planning and design of the technical, functional, and visual components of a website before it is finally developed and implemented.

The main objective of web architecture is to achieve the goal of solving each of the needs of a website in the best possible way. It is there for seeking a good user experience. The structure of the website should be logical, optimized, and efficient.

Web architecture is closely related to the Search Engine Optimization
(SEO). A simple, organized and coherently designed architecture facilitates the indexing and tracking of a website in search engines. Thus, SEO results depend exclusively on the quality of the structure and design of the website architecture.

Very often “less is better”!

## Monolithic architecture

Monolithic architecture describes buildings which are carved, cast, or excavated from a single piece of material, historically from rock. This is the traditional structure for software applications. Monolithic is an end-to-end architecture, in which all aspects of the software function as a single unit. 

Analysts often compare it to microservices, a newer model for application development. In the microservices model, components are modular, work independently, and are coupled together as needed for optimal functionality.

It has three components that interact with a single database:

   - Client-side user interface

   - Server-side application

   - Data interface

Software built according to this model works with a single code base. As a result, every time stakeholders want to make updates or changes, they access the same set of code. This can have a ripple effect that affects user-side performance.

This model can also streamline the ETL pipeline, as data flows into a single database through the monolith. However, even if you implement a microservices model, it can simplify your ETL significantly with a no-code solution.

This type of architecture is characterized by:

- **Ease**: programs are easy to develop.

- **Simplicity**: software deployment and execution are straightforward.

- **Affordable**: the development cost is low compared to other architectures.

The problems of this type of architecture, such as scalability or the difficulty for developers (they need to understand all the application code) have caused this type of software development to stop being used in many projects despite its advantages.

## Microservices architecture

Microservices architecture is a software application development method that works as a set of small services that run independently and autonomously, providing complete functionality. In it, each microservice is a code that can be in a different programming language, and that performs a specific function. 

Microservices communicate with each other through APIs and have their own storage systems which avoids overloading and crashing the application.

Advantages of implementing microservices architecture:

- **Maintainability**: the application can be divided into several functional and independent parts. In case you need to modify application functionality, only the affected component will be deployed.

- **Simultaneity**: while one team is busy developing one of the components, other teams can be performing maintenance or enhancements to other components without interruption.

- **Scalability**: this type of architecture has high scalability and ease of integration with third-party applications.

This model also has disadvantages such as the complexity of versioning or the problems of integration and development if there is little support or the high memory consumption involved in working with it.

## Layered or N-tier 

N-tier architecture is a client-server architecture concept in which data presentation, processing, and management functions are separated both logically and physically. 

Each of these functions runs on a separate machine or in separate clusters, so that each can provide services at its maximum capacity, since resources are not shared. This separation makes it easier to manage each of them in different layers, since work on one of them does not affect the others, isolating any problems that may arise.

N-Tiers architectures have at least 3 separate logical levels. Each layer has a specific functionality for which it is responsible and is located on different physical servers. A layer is deployed in a tier if more than one service or application is dependent on the functionality exposed by the layer. N-tier architecture is also known as multi-tier architecture.

Benefits provided by this architecture:

- **Availability**: applications can exploit the modular architecture using easily scalable components.

- **Flexibility**: each layer can be managed or scaled independently, which increases flexibility. 

- **Maintainability**: each layer is independent of the others. A layer can be updated or modified without affecting the application as a whole.  

- **Scalability**: it is reasonably easy to scale since the tiers are based on the deployment of the layers. 

The main disadvantages of implementing a layered architecture are the impediment to the deployment of functions that monolithic design entails and the complexity of network security management in a large system.

## Service-oriented architecture (SOA)

Service-Oriented Architecture, also known as SOA is a type of software architecture that allows the reuse of its elements thanks to service interfaces that communicate through a network with a common language. It defines the use of services (specific programs or tasks with a specific function) to support business requirements.  

SOA architecture makes it possible to integrate software elements that are implemented and maintained separately, allowing them to communicate with each other and work together to form software applications in different systems. Each SOA service is independent of the others and can be replaced or upgraded without breaking with the applications it connects.  

Services are distributable. They can be located anywhere on the network as long as it supports the required communication protocols.  In an SOA architecture, services share contracts and schemas when communicating, not internal classes.  They are as well policy-compliant, understanding policies as the definition of characteristics such as transport, protocol, or security.  

Advantages of using this model:

- **Efficiency**: processes are very efficient.

- **Maintainability**: Reduced maintenance costs.

- **Adaptability**: Facilitates adaptation to change, with integration with legacy systems.

- **Dynamics**: Encouragement of innovation oriented to the development of services, in line with market dynamism. Systems that are obsolete for economic, functional, or technical reasons are modernized.

- **Simple**: design is straightforward, optimizing organizational capacity.

The disadvantages of this architecture model are that without communication standards between applications, a lot of coding time is required. Applications with a high level of data transfer or with a short life span are not compatible with this model. At the level of protocols and services, it is arguably a more expensive system than others we have seen previously.

## Event-driven architecture

Event-driven architecture is a software model and architecture used to design applications. In such a system, the capture, communication, processing, and permanence of events are the core structure of the solution. This differs from the traditional request-based model.

But, what’s an event? Let’s go backwards…

Events are those significant changes in the state of a system's hardware or software. An event and its notification are not the same things: the latter is a message that the system sends to communicate to another part of the system that a certain event occurred.

Events can originate from internal or external stimuli. They can be generated by a user's activity, for example, when he clicks the mouse or presses a key; from an external source, as in the case of a sensor; or from the system, for instance, when a program is loaded.

This type of architecture is composed of event producers and event consumers. The former detects events and represents them as messages. It does so without knowing the event consumer or the result that the latter will generate. 

Once an event is detected, it is transmitted from the producer to the consumers through event channels. There it is processed asynchronously thanks to a platform for this purpose. When an event occurs, it must be reported to the consumers, who could process it or simply receive it. 

The processing platform will execute the appropriate response for the event and send the activity to the corresponding consumers. This downstream activity corresponds to where the result of the event will be seen. 

Benefits of event-driven architecture:

- **Scalability**: Scalability is one of the strongest points of this architecture since it allows each consumer to scale independently, thus reducing the coupling between components.

- **Deployment**: Due to the low coupling between components, deployment is possible without worrying about dependencies or preconditions.

- **Flexibility**: EDA allows rapid response to a changing environment, because each event processing component has a single responsibility and is completely decoupled from the others.

The most significant disadvantages associated with this model are the difficult testability of the tests, being an asynchronous model adds more complexity to this part. The lack of guarantee of obtaining a response to the sender and the scarcity of recovery support in case of partial failure are the most significant drawbacks.

Arguably its biggest handicap is the inability to predict when a request or reaction to an event will arrive; these could occur at any time. For this reason, it is often necessary to implement a queuing system at times of heavy traffic.

## ASYNCAPI and EDA

AsyncAPI is an open-source initiative that seeks to improve the current state of Event-Driven Architectures (EDA). Its long-term goal is to make working with EDAs as easy as it is to work with REST APIs. That goes from documentation to code generation, from discovery to event management. Most of the processes you apply to your REST APIs nowadays would be applicable to your event-driven asynchronous APIs too.

To make this happen, the first step has been to create a specification that allows developers, architects, and product managers to define the interfaces of an AsyncAPI. Much like OpenAPI (fka Swagger) does for REST APIs. 

The specification settles the base for a greater and better tooling ecosystem for EDA's. 

The event architecture allows you to create more accessible applications with less coupling between services, thus enabling a highly flexible architecture. These fundamental characteristics make this model the best choice for AsyncAPI development.

One of the reasons for the success of REST APIs has been the existence of standards like OpenAPI that allow you to edit specifications, create documentation automatically, mock generators, etc. And it is the contribution to this success that is the main driver of AsyncAPI. Currently, the strategy is to continue improving, implementing resources that make it more complete and solid. 

You might be looking for a solution to automate and formalize the documentation or code generation of your event-driven (micro)services. Likewise, you might be aiming to establish solid standards for your events and improve the governance of your asynchronous APIs. If so, AsyncAPI is here to help you.

Vice versa, we are looking forward to your feedback and contributions. If you have not yet joined the AsyncAPI community through its Slack or GitHub we invite you to participate in the growth of the specification.

See you in the next video!
