[Darlean](https://darlean.io) is an open source, cross-language library for creating regular and distributed backend applications. It eliminates much of the
complexity that comes with distributed scalable computing (like inter process comunnication, scalability, concurrency, deployment and persistence) so that
engineers can focus on the actual domain logic.

Darlean is created to solve the [microservice premium](https://martinfowler.com/bliki/MicroservicePremium.html). 
Instead of having to start a project as a complex (and expensive) 
microservice project on forehand because it may grow in the future, or to start a project as a simple monolith at the risk of having to perform an expensive
rewrite when scalability or availability actually become an issue, Darlean makes it possible to start simple and to scale out when necessary with
zero or minimal changes to your application.

The library provides:
* [Virtual actor](https://darlean.io/the-virtual-actor-model/) primitives that are well integrated with the supported programming languages (currently [TS/JS](https://github.com/darlean-io/darlean.ts) and [Go](https://github.com/darlean-io/darlean.go)).
* An [integrated high-performance message bus](https://darlean.io/documentation/configuration-options/#messaging-options) for inter-process communication (an external NATS message bus can also be configured).
* Integrated [scalable persistence](https://darlean.io/documentation/persistence/) (extendable architecture; external persistence providers can be used as well)
* Integrated [scalable indexed tables](https://darlean.io/documentation/tables/) (extendable architecture; external table services can be used as well)
* Integrated api gateways allow invocation of actors via HTTP/S.
* Persistent timers that invoke actors even when they are asleep.

# Features

## Efficient development
Darlean’s integration of the actor model with optional built-in persistence significantly boosts programming efficiency. Whether you’re building scalable or regular solutions, it accelerates development cycles, reducing the time and effort required to bring software projects to market.

## Scalable primitives
One standout feature is its comprehensive set of scalable primitives — storage, tables, queues, web gateways, and more — empowering developers to create scalable applications with reduced external dependencies.

## Language interoperability
Darlean simplifies the integration of multiple programming languages within a single application. This is particularly valuable when when leveraging different languages for specific components of a project. It currently includes a TypeScript library for Node.js, with libraries for .NET and Go scheduled for release in Q1 2024.

## Concurrent programming
Darlean provides tools and abstractions for handling concurrency, making it easier to write applications that efficiently execute multiple tasks or processes concurrently without the risk of race conditions or out-of-order messaging issues.

## Distributed programming
Darlean helps manage the complexities of building applications that run on distributed systems. It abstracts away low-level networking details, making it easier to develop software that spans multiple machines or nodes.

## Reduced provider dependency
By minimizing dependencies on specific service providers or infrastructure, Darlean enhances flexibility and portability. Developers can build applications that are less tied to particular cloud platforms or vendors, reducing vendor lock-in and facilitating easier migration.

## Open source
It is our passion to bring the paradigm of actor-oriented programming to a wide audience, because we believe that software development and deployment can — and should — be simple, even for complex, scalable solutions. That is why we provide Darlean free for anyone to use under the [Apache 2.0 License](https://www.apache.org/licenses/LICENSE-2.0).
