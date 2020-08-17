### Full Stack Serverless

Full Stack Serverless applications are applications that combine the following three things:

1. Decoupled frontends
2. Infrastructure as code
3. Serverless technologies for maximum scalability with minimum devops

By combining serverless technologies with end to end full stack example applications and reference architectures, developers are able to pick up, replicate, deploy to the cloud, and iterate on sophisticated scalable cloud applications in a way that, in the past, was not possible to do or accessible for the majority of developers.

Because many Serverless technologies like AWS Amplify, CDK, and the Serverless Framework (among others) are lowering the barrier to entry in building cloud applications with IAC (Infrastructure as Code), there is a new generation of traditionally front-end developers that can use their existing web and mobile skillset to build the types of applications that were traditionally out of their reach.

When I say use their existing skillset, I'm assuming that the typical front end or full stack developer is familiar with the following:

1. JavaScript, TypeScript, or Python
2. Interacting with a CLI
3. A basic understanding of interacting with RESTful and / or GraphQL APIS

Full Stack Serverlesss applications can be shared and deployed as an end to end project without much concern about the developer's local environment because all of the infrastructure is running in the cloud. They can be put down, shared, iterated on, and picked back up with ease.

Back end infrastructure can be created and destroyed within only a few minutes enabling developers to not have to worry about incurring much development cost. Because the services are Serverless, whatever development costs incurred will be low anyway.

#### The project

The [Full Stack Serverless project](https://github.com/full-stack-Serverless) is meant as a place for developers to get started with Full Stack Serverless applications by providing a variety of full stack reference architectures.

Applications need only to follow the three Full Stack Serverless criteria to be a part of this project.

This project is cloud agnostic. Azure, GCP, AWS, and any other cloud provider is welcome as long as they follow the above 4 principles.

Applications should be broken up into a front-end and back-end, with the following naming conventions:

__Back end / IAC__: IAC_PROVIDER-APP_NAME (i.e. cdk-appsync-chat)

__Front end__: FRAMEWORK_OR_PLATFORM-APP_NAME-CLOUD_INTEGRATION (i.e. react-chat-app-aws)

#### Why Serverless

Full Stack Serverless relies heavily on the Serverless philosophy for building out back end functionality. This means that the following are taken into consideration:

1. Developer velocity is valued above service ownership
2. Focus on creating business value vs re-inventing the wheel
3. Total cost of ownership should be understood at a fundamental level
4. Code is a liability
5. If it's available as a service, then it should never be built from scratch
6. Serverless functions fill in the gaps that managed services do not cover

Research also suggests that cloud computing is becoming more and more Serverless, meaning that Serverless is more future-proof than Serverful.

In [Cloud Programming Simplified: A Berkeley View on Serverless Computing](https://www2.eecs.berkeley.edu/Pubs/TechRpts/2019/EECS-2019-3.pdf), the predictions for the future of cloud computing were this:

- We expect new BaaS storage services to be created that expand the types of applications that
run well on Serverless computing. Such storage will match the performance of local block
storage and come in ephemeral and durable variants. We will see much more heterogeneity of
computer hardware for Serverless computing than the conventional x86 microprocessor that
powers it today.
- We expect Serverless computing to become simpler to program securely than Serverful computing, benefiting from the high level of programming abstraction and the fine-grained isolation
of cloud functions.
- We see no fundamental reason why the cost of Serverless computing should be higher than
that of Serverful computing, so we predict that billing models will evolve so that almost
any application, running at almost any scale, will cost no more and perhaps much less with
Serverless computing.
- The future of Serverful computing will be to facilitate BaaS. Applications that prove to be
difficult to write on top of Serverless computing, such as OLTP databases or communication
primitives such as queues, will likely be offered as part of a richer set of services from all cloud
providers.
- While Serverful cloud computing won’t disappear, the relative importance of that portion of
the cloud will decline as Serverless computing overcomes its current limitations.
- Serverless computing will become the default computing paradigm of the Cloud Era, largely
replacing Serverful computing and thereby bringing closure to the Client-Server Era.

In the above paper they redefined the term __Serverless__ to be this:

> Put simply, Serverless computing = FaaS + BaaS.

The definition of Serverless is no longer only Functions as a service, but now also encompasses backends as a service (Baas).

In addition to the traditional advantages of Serverless technologies, there is another main reason why Serverless technologies are preferred over Serverful for this project:

__Lower barrier to entry for traditionally non-back-end developers__

Because developers are leveraging managed services for functionality like authenticaiton and databases and not having to manage infrastruture, it is a lower barrier to entry for new developers than traditional Serverful cloud computing.