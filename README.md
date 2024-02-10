
# Microservices Architecture

## 1. What are Microservices?

<img src="https://microservices.io/i/Microservice_Architecture.png" alt="" width="auto" height="auto" />



<img src="" alt="" width="auto" height="auto" />

Microservices are an architectural approach to building software applications as a collection of small, independently deployable services. Each service is self-contained and focused on a specific business capability, running its process and communicating with lightweight mechanisms, often an HTTP-based API.

## 2. Difference between Monolithic and Microservices

### Monolithic Architecture
In a monolithic architecture, the entire application is built as a single, indivisible unit. All functionalities, such as user interface, business logic, and data access, are tightly coupled within the same codebase.

<img src="https://miro.medium.com/v2/resize:fit:755/1*Tiizur0VlvZlJSIgADsp4w.png" alt="" width="auto" height="auto" />

### Microservices Architecture
Microservices architecture breaks down the application into smaller, loosely coupled services. Each service is responsible for a distinct function and can be developed, deployed, and scaled independently. This approach offers flexibility, scalability, and easier maintenance compared to monolithic architecture.

<img src="https://miro.medium.com/v2/resize:fit:937/1*Jn_OZgq9dAG854kLEvG_-Q.png" alt="" width="auto" height="auto" />

## 3. Data Management in Microservices

Data management in microservices involves handling data within each service and coordinating data flow between services.

## 4. Database per Service

### Issues
- **Uptime Increase Issue:** Each service having its own database can lead to increased uptime requirements for maintaining multiple databases.
- **Database Schema Changes Issue:** Changes to one service's database schema may impact other services that depend on it.
- **Features Require Different Databases Issue:** Some features may require different types of databases, which complicates the architecture.

## 5. Challenges in Data Management Services

Managing data in a microservices architecture presents various challenges including:
- Data consistency across services
- Synchronization of data updates
- Versioning and compatibility of data schemas
- Data access patterns and performance optimization

## 6. Methodologies: Sync and Async

### Synchronous Communication
In synchronous communication, services communicate directly with each other, typically over HTTP. This approach is straightforward but can lead to tight coupling and performance issues.

<img src="https://www.researchgate.net/publication/350005223/figure/fig2/AS:1000372491522048@1615518796091/Synchronous-and-Asynchronous-communication-schemes-between-microservices.ppm" alt="" width="auto" height="auto" />

### Asynchronous Communication
In asynchronous communication, services communicate indirectly through message brokers or event buses. This decouples services and improves scalability and fault tolerance, but adds complexity in handling eventual consistency and message delivery guarantees.


<img src="https://learn.microsoft.com/en-us/dotnet/architecture/microservices/architect-microservice-container-applications/media/asynchronous-message-based-communication/asynchronous-event-driven-communication.png" alt="" width="auto" height="auto" />


## Resources

1. [Microservice architecture information](https://microservices.io/index.html)
