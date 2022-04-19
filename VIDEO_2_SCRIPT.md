
## Video 2: What kinds of API architectures exist

- Synchronous and asynchronous APIs
- API Architecture definition
- Types of APIs architecture

   - Monolithic
   - Microservices
   - Serverless
   - Event-driven
    
-	EDA and AsyncAPI

Hello everyone! Welcome!

In this video, we're going to talk about the different types of API architectures that exist. We'll try to explain their meaning, discover what they bring, what they're used for, and how to analyze them. If after listening to explanation of different architectures you find it all making things super complex, sorry, but it is even more complex as you can mix them all together.

Let's start with web architectures!

## Synchronous and asynchronous APIs

APIs can follow two communication models. Synchronous or asynchronous communication. Let's see what they consist of and how they differ:

Synchronous APIs allow the exchange of information in real-time between two machines, such as a videoconference or a phone call. The participants have to be connected at the same time.

Asynchronous APIs have been gaining strength in recent years. This type of API allows the exchange of information between machines in a non-simultaneous way, the participants do not have to be connected at the same time. Communication can be done individually or collectively, as in web forums or e-mail. It is also faster and cheaper than synchronous APIs since they make more optimal use of the hardware for their operation.

## API Architecture definition

API architecture is the process of defining the methodology, development, and implementation of APIs. It results in a set of components and a description of their logical interaction.

Once the methodology to be worked with has been defined, the operations and security teams shape the specific technical requirements that will describe the future of the API. Another crucial point developed by them is the tiers, API lifecycle management, and API profitability.

## Types of APIs architecture

### Monolithic architecture

Monolithic architecture describes buildings which are carved, cast, or excavated from a single piece of material, historically from rock. This is the traditional structure for software applications. Monolithic is an end-to-end architecture, in which all aspects of the software function as a single unit. 

Analysts often compare it to microservices, a newer model for application development. In the microservices model, components are modular, work independently, and are coupled together as needed for optimal functionality.

Monolithic architecture has three components that interact with a single database:

   - Client-side user interface

   - Server-side application

   - Data interface

Software built according to this model works with a single code base. As a result, every time stakeholders want to make updates or changes, they access the same set of code. This can have a ripple effect that affects user-side performance.

This model can also streamline the ETL pipeline, as data flows into a single database through the monolith. However, even if you implement a microservices model, it can simplify your ETL significantly with a no-code solution.

This type of architecture is characterized by:

- **Ease**: programs are easy to develop.

- **Simplicity**: software deployment and execution are straightforward.

- **Affordable**: the development cost is low compared to other architectures.

Some of the problems with this type of architecture are scalability and onboarding difficulty for developers. This has caused this type of software development to stop being used in many projects despite its advantages.

### Microservices architecture

Microservices architecture is a software application development method that works as a set of small services that run independently and autonomously, providing complete functionality. In it, each microservice is a code that can be in a different programming language, and that performs a specific function. 

Microservices communicate with each other through APIs and have their own storage systems which avoids overloading and crashing the application.

Let's talk about some advantages of implementing microservices architecture:

- **Maintainability**: the application can be divided into several functional and independent parts. In case you need to modify application functionality, only the affected component will be deployed.

- **Simultaneity**: while one team is busy developing one of the components, other teams can be performing maintenance or enhancements to other components without interruption.

- **Scalability**: this type of architecture has high scalability and ease of integration with third-party applications.

This model also has disadvantages such as the complexity of versioning, problems with integration and development, little support, and the high memory consumption involved in working with it.

### Serverless architecture

It is a computing model that uses the cloud as the environment for executing applications and processes, dispensing with traditional servers. In Serverless, services are managed by the FaaS (Function as a Service) service provider.

In this way, the Serverless architecture facilitates the work of developers, as they can dispense with tasks such as the allocation of server resources. With Serverless, the code runs directly in containers. The organization is external to the developers, who only have to pay the FaaS provider for the time of use of its services.

Let's see what advantages this type of architecture offers us:
 
- **Scalability**: in terms of growth and decrease. If service usage drops during a specific period, costs are adjusted by not assuming the costs of hibernation periods if extra capacity is needed at a given moment.

- **Efficiency**: saves costs both in infrastructure and human resources. Developers work exclusively on programming new functionalities. 

- **Flexibility**: its system favors autonomy and experimentation without the obligation to involve a large number of actors or to make a high investment.

The main disadvantages of using this type of architecture are the great initial effort to adapt the organization's structures in the implementation phase and the dependence on the FaaS provider, which in the long term may hinder the changeover by having to modify the programming languages and functions used to meet the requirements of the new Serverless service provider.

### Event-driven architecture

Event-driven architecture is a software model and architecture used to design applications. In such a system, the capture, communication, processing, and permanence of events are the core structure of the solution. This differs from the traditional request-based model.

But, what’s an event? Let’s go backwards…

Events are those significant changes in the state of a system's hardware or software. An event and its notification are not the same things: the latter is a message that the system sends to communicate to another part of the system that a certain event occurred.

Events can originate from internal or external sources. They can be generated by a user's activity, for example, when users click the mouse or press a key; from an external source, as in the case of a sensor; or from the system, for instance, when a program is loaded.

This type of architecture is composed of event producers and event consumers. The former detects events and represents them as messages. It does so without knowing the event consumer or the result that the latter will generate. 

Once an event is detected, it is transmitted from the producer to the consumers through event channels. There it is processed asynchronously thanks to a platform for this purpose. When an event occurs, it must be reported to the consumers, who could process it or simply receive it. 

The processing platform will execute the appropriate response for the event and send the activity to the corresponding consumers. This downstream activity corresponds to where the result of the event will be seen. 

Let's discuss the benefits of event-driven architecture:

- **Scalability**: Scalability is one of the strongest points of this architecture since it allows each consumer to scale independently, thus reducing the coupling between components.

- **Deployment**: Due to the low coupling between components, deployment is possible without worrying about dependencies or preconditions.

- **Flexibility**: EDA allows rapid response to a changing environment, because each event processing component has a single responsibility and is completely decoupled from the others.

The most significant disadvantages associated with this model are the difficult testability of the tests. Being an asynchronous model adds more complexity to this part. The lack of guarantee of obtaining a response to the sender and the scarcity of recovery support in case of partial failure is the most significant drawback.

Arguably its biggest handicap is the inability to predict when a request or reaction to an event will arrive; these could occur at any time. For this reason, it is often necessary to implement a queuing system at times of heavy traffic.

## ASYNCAPI and EDA

AsyncAPI is an open-source initiative that seeks to improve the current state of Event-Driven Architectures (EDA). Its long-term goal is to make working with EDAs as easy as it is to work with REST APIs. That goes from documentation to code generation and from discovery to event management. Most of the processes you apply to your REST APIs nowadays would be applicable to your event-driven asynchronous APIs too.

To make this happen, the first step has been to create a specification that allows developers, architects, and product managers to define the interfaces of the EDA interfaces using AsyncAPI. Much like OpenAPI (fka Swagger) does for REST APIs. 

The specification settles the base for a greater and better tooling ecosystem for EDA's. 

The event architecture allows you to create more accessible applications with less coupling between services, thus enabling a highly flexible architecture. These fundamental characteristics make this model the best choice for AsyncAPI development.

One of the reasons for the success of REST APIs has been the existence of standards like OpenAPI that allow you to edit specifications, create documentation automatically, mock generators, etc. And it is the contribution to this success that is the main driver of AsyncAPI. Currently, the strategy is to continue improving, implementing resources that make it more complete and solid. 

You might be looking for a solution to automate and formalize the documentation or code generation of your event-driven (micro)services. Likewise, you might be aiming to establish solid standards for your events and improve the governance of your asynchronous APIs. If so, AsyncAPI is here to help you.

Vice versa, we are looking forward to your feedback and contributions. If you have not yet joined the AsyncAPI community through its Slack or GitHub Discussions, we invite you to participate in the growth of the specification.

See you in the next video!