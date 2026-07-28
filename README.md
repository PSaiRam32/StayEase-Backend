<p align="center">
  <img src="StayEase.png" alt="StayEase Banner" width="100%">
</p>

# 🏨 StayEase – Hostel & PG Booking Platform

<div align="center">


![Java](https://img.shields.io/badge/Java-21-orange?style=for-the-badge)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-3.x-brightgreen?style=for-the-badge)
![Spring Cloud](https://img.shields.io/badge/Spring_Cloud-Microservices-success?style=for-the-badge)
![Gradle](https://img.shields.io/badge/Gradle-Build_Tool-02303A?style=for-the-badge&logo=gradle)
![MySQL](https://img.shields.io/badge/MySQL-Database-blue?style=for-the-badge&logo=mysql)
![JWT](https://img.shields.io/badge/JWT-Security-black?style=for-the-badge&logo=jsonwebtokens)
![OpenFeign](https://img.shields.io/badge/OpenFeign-Service_Communication-lightgrey?style=for-the-badge)
![Razorpay](https://img.shields.io/badge/Razorpay-Payments-02042B?style=for-the-badge&logo=razorpay)
![Status](https://img.shields.io/badge/Status-Active-success?style=for-the-badge)

</div>

# 📑 Table of Contents

- [📖 Project Overview](#-project-overview)
- [🎯 Business Problem](#-business-problem)
- [💡 Business Solution](#-business-solution)
- [🏛 Enterprise Concepts Demonstrated](#-enterprise-concepts-demonstrated)
- [🎯 Project Objectives](#-project-objectives)
- [✨ Major Features](#-major-features)
- [🛠 Technology Stack](#-technology-stack)
- [🚀 Future Technology Roadmap](#-future-technology-roadmap)
- [🌟 Platform Highlights](#-platform-highlights)
- [🏗 High-Level System Architecture](#-high-level-system-architecture)
- [🧩 Microservices Overview](#-microservices-overview)
- [📋 Service Responsibilities](#-service-responsibilities)
- [🔄 End-to-End Request Flow](#-end-to-end-request-flow)
- [🌐 Inter-Service Communication](#-inter-service-communication)
- [🗄 Database per Service Architecture](#-database-per-service-architecture)
- [🔗 External Integrations](#-external-integrations)
- [🔄 End-to-End Business Workflows](#-end-to-end-business-workflows)
  - [👤 User Registration Workflow](#-user-registration-workflow)
  - [🔐 Login & Authentication Workflow](#-login--authentication-workflow)
  - [📧 Email Verification Workflow](#-email-verification-workflow)
  - [🏠 Property Discovery Workflow](#-property-discovery-workflow)
  - [📅 Booking Workflow](#-booking-workflow)
  - [💳 Payment Workflow](#-payment-workflow)
  - [📧 Notification Workflow](#-notification-workflow)
  - [❌ Booking Cancellation Workflow](#-booking-cancellation-workflow)
  - [💰 Refund Workflow](#-refund-workflow)
  - [🏢 Owner Management Workflow](#-owner-management-workflow)
  - [🌐 Platform Collaboration Overview](#-platform-collaboration-overview)
- [🏛 Enterprise Architecture Decisions](#-enterprise-architecture-decisions)
  - [🌐 Why Microservices?](#-why-microservices)
  - [🚪 Why API Gateway?](#-why-api-gateway)
  - [🗄 Why Database per Service?](#-why-database-per-service)
  - [🔐 Why JWT Authentication?](#-why-jwt-authentication)
  - [📡 Why OpenFeign?](#-why-openfeign)
  - [💳 Why a Dedicated Payment Service?](#-why-a-dedicated-payment-service)
  - [📧 Why a Dedicated Notification Service?](#-why-a-dedicated-notification-service)
  - [🏗 Why Layered Architecture?](#-why-layered-architecture)
  - [🔄 Why Transaction Management?](#-why-transaction-management)
  - [🛡 Security Principles](#-security-principles)
  - [🚀 Production Readiness](#-production-readiness)
  - [🌟 Architectural Principles](#-architectural-principles)
- [📂 Repository Structure](#-repository-structure)
- [🔗 Service Repositories](#-service-repositories)
- [🚀 Getting Started](#-getting-started)
- [📮 API Documentation](#-api-documentation)
- [🤝 Contributing](#-contributing)
- [📜 License](#-license)
- [👨‍💻 Author](#-author)
---

# 📖 Project Overview

**StayEase** is an enterprise-grade accommodation booking platform built using **Java 21**, **Spring Boot**, **Spring Cloud Microservices**, **MySQL**, **Spring Security**, and **Gradle**.

The platform enables users to discover, book, and manage accommodations while allowing property owners to manage listings, monitor bookings, and track business performance through dedicated dashboards.

Unlike traditional monolithic booking systems, StayEase follows a **Microservices Architecture**, where every business capability is implemented as an independent service with its own database, business logic, and deployment lifecycle.

The platform demonstrates modern enterprise backend engineering practices including:

- Microservices Architecture
- API Gateway Pattern
- Database per Service Pattern
- JWT Authentication & Authorization
- Email Verification
- Refresh Token Authentication
- Secure Password Management
- OpenFeign Inter-Service Communication
- Circuit Breaker & Retry Mechanisms
- Layered Architecture
- Domain-Driven Design (DDD)
- Spring Security
- Bean Validation
- Global Exception Handling
- Asynchronous Notification Processing
- Payment Gateway Integration (Razorpay)

The architecture has been designed to support future enterprise enhancements including:

- Apache Kafka Event-Driven Communication
- Docker & Docker Compose
- Kubernetes
- Prometheus & Grafana
- Centralized Logging
- Distributed Tracing
- CI/CD Pipelines
- Cloud Deployment (AWS / Azure / GCP)

---

# 🎯 Business Problem

Traditional accommodation booking systems often rely on tightly coupled architectures where authentication, property management, booking, payments, and notifications are implemented within a single application.

Such systems commonly face several challenges:

- Limited scalability as the application grows.
- Tight coupling between business modules.
- Difficult independent deployment of features.
- Single points of failure affecting the entire platform.
- Poor maintainability due to increasing code complexity.
- Limited fault isolation between business domains.
- Challenges integrating new services and technologies.

As user traffic increases, these limitations negatively impact system performance, reliability, and long-term maintainability.

---

# 💡 Business Solution

StayEase addresses these challenges by adopting a modern **Spring Boot Microservices Architecture**.

Each business capability is implemented as an independent microservice responsible for its own business logic and data ownership.

Current services include:

- API Gateway
- Authentication Service
- User Service
- Owner Service
- Property Service
- Booking Service
- Payment Service
- Notification Service

This architecture provides:

- Independent service deployment
- Database per Service
- Improved scalability
- Better fault isolation
- Easier maintenance
- Clear business boundaries
- Simplified future expansion
- Production-oriented architecture

By separating responsibilities across dedicated services, StayEase achieves a scalable, maintainable, and enterprise-ready backend platform capable of supporting future growth and advanced cloud-native capabilities.

---

# 🏛 Enterprise Concepts Demonstrated

StayEase has been designed by following modern enterprise software engineering principles commonly used in large-scale distributed systems.

The project demonstrates practical implementation of the following concepts:

- Microservices Architecture
- API Gateway Pattern
- Database per Service Pattern
- Domain-Driven Design (DDD)
- Layered Architecture
- Spring Security
- JWT Authentication & Authorization
- Refresh Token Authentication
- Email Verification
- Password Encryption (BCrypt)
- Role-Based Access Control (RBAC)
- OpenFeign Inter-Service Communication
- Circuit Breaker Pattern
- Retry Mechanism
- Bean Validation
- Global Exception Handling
- Transaction Management
- Secure Payment Integration (Razorpay)
- Asynchronous Notification Processing
- RESTful API Design
- Environment-Based Configuration
- Enterprise Logging
- Production-Oriented Project Structure

The architecture has also been intentionally designed to support future migration toward an event-driven and cloud-native ecosystem.

---

# 🎯 Project Objectives

StayEase was developed to simulate how a real-world accommodation booking platform would be designed using enterprise backend development practices.

The primary objectives of the project include:

- Build a scalable microservices-based booking platform.
- Separate business domains into independently deployable services.
- Implement secure authentication and authorization.
- Demonstrate enterprise-grade REST API development.
- Integrate online payment processing.
- Provide reliable notification delivery.
- Maintain clear service ownership and database isolation.
- Follow clean architecture and SOLID principles.
- Prepare the platform for future cloud-native deployment.

Beyond implementing business functionality, the project also serves as a practical demonstration of production-oriented software architecture.

---

# ✨ Major Features

StayEase consists of multiple business domains working together to provide a complete accommodation booking experience.

## 🔐 Authentication & Security

- User Registration
- Owner Registration
- Secure Login
- JWT Authentication
- Refresh Token Authentication
- Email Verification
- Forgot Password
- Password Reset
- Logout
- BCrypt Password Encryption
- Role-Based Access Control

---

## 👤 User Management

- User Profile Management
- Profile Picture Upload
- Wishlist Management
- Booking History
- Account Management

---

## 🏢 Owner Management

- Owner Dashboard
- Property Management
- Booking Overview
- Revenue Summary
- Occupancy Statistics

---

## 🏠 Property Management

- Property Registration
- Property Approval Workflow
- Room Management
- Amenities Management
- Property Search
- Property Reviews & Ratings
- Availability Information

---

## 📅 Booking Management

- Property Booking
- Dynamic Availability Calculation
- Booking History
- Booking Cancellation
- Booking Rescheduling
- Check-In & Check-Out Management

---

## 💳 Payment Management

- Razorpay Order Creation
- Secure Payment Verification
- Payment Status Tracking
- Refund Processing
- Receipt Generation
- Payment Retry
- Audit Logging

---

## 📧 Notification Management

- Email Notifications
- Asynchronous Processing
- Automatic Retry
- Exponential Backoff
- Duplicate Notification Detection
- Notification History
- Notification Status Tracking

---

# 🛠 Technology Stack

| Category | Technology |
|------------|------------|
| Language | Java 21 |
| Framework | Spring Boot |
| Microservices | Spring Cloud |
| API Gateway | Spring Cloud Gateway |
| Security | Spring Security, JWT |
| Database | MySQL |
| ORM | Spring Data JPA, Hibernate |
| Build Tool | Gradle |
| Service Communication | OpenFeign |
| Fault Tolerance | Resilience4j |
| Payment Gateway | Razorpay |
| Email | JavaMailSender |
| Validation | Jakarta Bean Validation |
| Documentation | Swagger / OpenAPI |
| Logging | SLF4J |
| Version Control | Git & GitHub |

---

# 🚀 Future Technology Roadmap

The platform has been architected to support additional enterprise technologies with minimal refactoring.

Future enhancements include:

| Category | Planned Technology |
|------------|-------------------|
| Event Streaming | Apache Kafka |
| Containerization | Docker & Docker Compose |
| Container Orchestration | Kubernetes |
| Monitoring | Spring Boot Actuator |
| Metrics | Prometheus |
| Dashboards | Grafana |
| Distributed Tracing | OpenTelemetry & Zipkin |
| Centralized Logging | ELK Stack / Loki |
| CI/CD | GitHub Actions |
| Cloud Deployment | AWS / Azure / GCP |

---

# 🌟 Platform Highlights

✔ Enterprise Microservices Architecture

✔ Eight Independent Microservices

✔ API Gateway

✔ JWT Authentication

✔ Refresh Token Security

✔ Email Verification

✔ Database per Service

✔ Razorpay Payment Integration

✔ Asynchronous Notification Processing

✔ OpenFeign Service Communication

✔ Circuit Breaker & Retry Mechanisms

✔ Enterprise Documentation

✔ Cloud-Native Ready Architecture
---
---

# 🏗 High-Level System Architecture

StayEase follows a **Microservices Architecture**, where each business domain is implemented as an independent service with its own business logic, database, and deployment lifecycle.

All external requests enter the platform through the **API Gateway**, which acts as the single entry point for routing, authentication, and request forwarding.

Business services communicate through secure REST APIs using **OpenFeign**, while each service maintains full ownership of its own data following the **Database per Service** pattern.

Future versions of the platform will extend this architecture with **Apache Kafka** to support asynchronous event-driven communication.

```mermaid
flowchart TB

Client["Web / Mobile Client"]

Gateway["API Gateway"]

Auth["Auth Service"]
User["User Service"]
Owner["Owner Service"]
Property["Property Service"]
Booking["Booking Service"]
Payment["Payment Service"]
Notification["Notification Service"]

AuthDB[(Auth DB)]
UserDB[(User DB)]
OwnerDB[(Owner DB)]
PropertyDB[(Property DB)]
BookingDB[(Booking DB)]
PaymentDB[(Payment DB)]
NotificationDB[(Notification DB)]

Razorpay["Razorpay"]
SMTP["SMTP Mail Server"]

Client --> Gateway

Gateway --> Auth
Gateway --> User
Gateway --> Owner
Gateway --> Property
Gateway --> Booking
Gateway --> Payment
Gateway --> Notification

Auth --> AuthDB
User --> UserDB
Owner --> OwnerDB
Property --> PropertyDB
Booking --> BookingDB
Payment --> PaymentDB
Notification --> NotificationDB

Payment --> Razorpay
Notification --> SMTP
```

---

# 🧩 Microservices Overview

StayEase is composed of eight independent microservices, each responsible for a specific business capability.

| Service | Primary Responsibility |
|----------|------------------------|
| API Gateway | Entry point, routing, request forwarding |
| Auth Service | Authentication, authorization, JWT, refresh tokens, email verification |
| User Service | User profile management, wishlist, booking history |
| Owner Service | Owner dashboard, property ownership, revenue insights |
| Property Service | Property management, rooms, amenities, search, reviews |
| Booking Service | Booking lifecycle, availability calculation, cancellations |
| Payment Service | Razorpay integration, payment verification, refunds |
| Notification Service | Email notifications, retries, notification history |

Each service can evolve, scale, and be deployed independently without affecting the rest of the platform.

---

# 📋 Service Responsibilities

## 🌐 API Gateway

Responsibilities:

- Single Entry Point
- Request Routing
- Authentication Forwarding
- Centralized Access
- Future Rate Limiting
- Future API Versioning

---

## 🔐 Auth Service

Responsibilities:

- User Authentication
- Owner Authentication
- JWT Generation
- Refresh Token Management
- Email Verification
- Forgot Password
- Password Reset
- Logout
- Role Management

---

## 👤 User Service

Responsibilities:

- User Profile Management
- Wishlist Management
- Booking History
- Profile Picture Upload
- Account Management

---

## 🏢 Owner Service

Responsibilities:

- Owner Dashboard
- Property Ownership
- Booking Monitoring
- Revenue Summary
- Occupancy Statistics

---

## 🏠 Property Service

Responsibilities:

- Property CRUD
- Room Management
- Amenities
- Property Approval
- Search & Filtering
- Reviews & Ratings

---

## 📅 Booking Service

Responsibilities:

- Booking Creation
- Dynamic Availability Calculation
- Booking Cancellation
- Booking Rescheduling
- Check-In
- Check-Out
- Booking History

---

## 💳 Payment Service

Responsibilities:

- Razorpay Order Creation
- Payment Verification
- Refund Processing
- Payment History
- Receipt Generation
- Audit Logging

---

## 📧 Notification Service

Responsibilities:

- Email Notifications
- Async Processing
- Automatic Retry
- Exponential Backoff
- Duplicate Detection
- Notification Tracking

---

# 🔄 End-to-End Request Flow

Every client request follows a structured processing pipeline before reaching the appropriate business service.

```mermaid
flowchart LR

Client["👤 Client"]

Gateway["🌐 API Gateway"]

Auth["🔐 Authentication"]

Service["🏢 Business Service"]

Logic["⚙️ Business Logic"]

DB[("🗄 Database")]

Response["📤 Response"]

Client --> Gateway

Gateway --> Auth

Auth --> Service

Service --> Logic

Logic --> DB

DB --> Logic

Logic --> Response

Response --> Client
```

This centralized request flow simplifies security, routing, and future platform expansion.

---

# 🌐 Inter-Service Communication

Business services communicate using **OpenFeign**, enabling synchronous REST-based interactions while keeping service boundaries clearly defined.

Current communication includes:

```mermaid
flowchart TD

Auth["🔐 Auth Service"]

User["👤 User Service"]

Owner["🏢 Owner Service"]

Property["🏠 Property Service"]

Booking["📅 Booking Service"]

Payment["💳 Payment Service"]

Notification["📧 Notification Service"]

Auth --> User
Auth --> Owner

Property --> Owner

Booking --> User
Booking --> Property
Booking --> Owner
Booking --> Payment
Booking --> Notification

Payment --> Booking
Payment --> Notification
```

Future versions will gradually introduce **Apache Kafka** for asynchronous event-driven communication where appropriate.

---

# 🗄 Database per Service Architecture

Each microservice owns its own dedicated database.

This architecture prevents tight coupling while allowing independent schema evolution and service scalability.

```mermaid
flowchart LR

Auth["🔐 Auth Service"] --> AuthDB[(Auth DB)]

User["👤 User Service"] --> UserDB[(User DB)]

Owner["🏢 Owner Service"] --> OwnerDB[(Owner DB)]

Property["🏠 Property Service"] --> PropertyDB[(Property DB)]

Booking["📅 Booking Service"] --> BookingDB[(Booking DB)]

Payment["💳 Payment Service"] --> PaymentDB[(Payment DB)]

Notification["📧 Notification Service"] --> NotificationDB[(Notification DB)]
```

Benefits of this approach include:

- Independent data ownership
- Loose coupling
- Better fault isolation
- Independent database scaling
- Easier schema evolution
- Improved service autonomy

---

# 🔗 External Integrations

StayEase integrates with external services to provide secure payment processing and reliable communication.

| External System | Purpose |
|-----------------|---------|
| Razorpay | Online payment processing |
| SMTP Server | Email notifications |

The architecture has also been prepared for future integrations such as Kafka, Redis, cloud storage providers, and monitoring platforms.

---

# 🔄 End-to-End Business Workflows

StayEase is composed of multiple independent microservices that collaborate to deliver a seamless accommodation booking experience.

Each workflow below illustrates how different services interact to accomplish a specific business operation while maintaining clear separation of responsibilities.

---

# 👤 User Registration Workflow

When a new user registers, the Authentication Service validates the request, creates authentication credentials, sends an email verification link, and provisions the corresponding user profile.

```mermaid
flowchart LR

A["👤 User"] --> B["🌐 API Gateway"]

B --> C["🔐 Auth Service"]

C --> D["Validate Registration Request"]

D --> E["Encrypt Password"]

E --> F["Generate Email Verification Token"]

F --> G["Persist Authentication Details"]

G --> H["📧 Notification Service"]

H --> I["Send Verification Email"]

G --> J["👤 User Service"]

J --> K["Create User Profile"]

K --> L["✅ Registration Completed"]
```

### Workflow Summary

- User submits registration details.
- API Gateway routes the request to the Authentication Service.
- Credentials are validated and securely stored.
- Password is encrypted using BCrypt.
- Email verification token is generated.
- Verification email is sent asynchronously.
- User profile is created in the User Service.
- Registration completes successfully.

---

# 🔐 Login & Authentication Workflow

After successful registration and email verification, users authenticate using their credentials to receive JWT tokens.

```mermaid
flowchart LR

A["👤 User"]

--> B["🌐 API Gateway"]

B --> C["🔐 Auth Service"]

C --> D["Validate Email & Password"]

D --> E{"Credentials Valid?"}

E -- No --> F["❌ Authentication Failed"]

E -- Yes --> G["Generate JWT Access Token"]

G --> H["Generate Refresh Token"]

H --> I["Return Authentication Response"]

I --> J["💻 Client Stores Tokens"]

J --> K["Future Requests Include JWT"]
```

### Workflow Summary

- User submits login credentials.
- Authentication Service validates credentials.
- JWT Access Token is generated.
- Refresh Token is generated.
- Tokens are returned to the client.
- Future API requests use the Access Token for authorization.

---

# 📧 Email Verification Workflow

Email verification ensures that only verified users can activate their accounts and access secured platform features.

```mermaid
flowchart LR

A["👤 User Registration"]

--> B["🔐 Auth Service"]

B --> C["Generate Verification Token"]

C --> D["📧 Notification Service"]

D --> E["Send Verification Email"]

E --> F["👤 User Clicks Verification Link"]

F --> G["🔐 Auth Service"]

G --> H["Validate Verification Token"]

H --> I{"Token Valid?"}

I -- No --> J["❌ Verification Failed"]

I -- Yes --> K["Activate Account"]

K --> L["Update Email Verified Status"]

L --> M["✅ Account Activated"]
```

### Workflow Summary

- Verification token is generated during registration.
- Notification Service sends the email.
- User clicks the verification link.
- Authentication Service validates the token.
- User account is activated.
- Email verification status is updated.

---

# 🏠 Property Discovery Workflow

Users can search for accommodations based on location, availability, amenities, pricing, and other business filters.

```mermaid
flowchart LR

A["👤 User"]

--> B["🌐 API Gateway"]

B --> C["🏠 Property Service"]

C --> D["Validate Search Criteria"]

D --> E["Apply Search Filters"]

E --> F["Retrieve Matching Properties"]

F --> G["Sort & Paginate Results"]

G --> H["Return Property Listings"]

H --> I["✅ Display Results"]
```

### Workflow Summary

- User searches for accommodations.
- Property Service validates search parameters.
- Filters are applied.
- Matching properties are retrieved.
- Results are sorted and paginated.
- Available properties are returned to the client.

---

# 📌 Key Design Principles Demonstrated

These workflows highlight several enterprise software engineering practices adopted throughout StayEase:

- Microservices Architecture
- API Gateway Pattern
- Layered Architecture
- Database per Service Pattern
- Secure Authentication using JWT
- Email Verification
- Asynchronous Notification Processing
- Loose Coupling Between Services
- Single Responsibility Principle
- Domain-Driven Design (DDD)

Each business capability remains isolated within its own service, enabling independent development, deployment, scalability, and maintenance.

---

# 📅 Booking Workflow

Booking a property is one of the core business processes in StayEase. It involves collaboration between multiple microservices to validate the request, calculate availability, create the booking, and initiate payment.

```mermaid
flowchart LR

A["👤 User"]
--> B["🌐 API Gateway"]

B --> C["📅 Booking Service"]

C --> D["Validate Booking Request"]

D --> E["🏠 Property Service"]

E --> F["Retrieve Property Details"]

F --> G["Calculate Room Availability"]

G --> H{"Room Available?"}

H -- No --> I["❌ Booking Rejected"]

H -- Yes --> J["Create Booking"]

J --> K["💳 Payment Service"]

K --> L["Generate Razorpay Order"]

L --> M["Return Payment Details"]

M --> N["✅ Booking Created"]
```

### Workflow Summary

- User submits a booking request.
- Booking Service validates booking details.
- Property Service provides room information.
- Booking Service calculates dynamic availability.
- Booking record is created.
- Payment Service generates a Razorpay order.
- Booking waits for payment confirmation.

---

# 💳 Payment Workflow

Once the booking is created, the Payment Service securely processes the payment using Razorpay.

```mermaid
flowchart LR

A["👤 User"]

--> B["💳 Razorpay Checkout"]

B --> C["💳 Payment Service"]

C --> D["Verify Payment Signature"]

D --> E{"Payment Verified?"}

E -- No --> F["❌ Payment Failed"]

E -- Yes --> G["Update Payment Status"]

G --> H["📅 Booking Service"]

H --> I["Confirm Booking"]

I --> J["📧 Notification Service"]

J --> K["Send Booking Confirmation"]

K --> L["✅ Booking Confirmed"]
```

### Workflow Summary

- User completes payment through Razorpay.
- Payment Service verifies the payment signature.
- Booking status is updated.
- Notification Service sends confirmation email.
- Booking becomes confirmed.

---

# 📧 Notification Workflow

Notification delivery is completely independent from business services to improve reliability and responsiveness.

```mermaid
flowchart LR

A["Business Service"]

--> B["📧 Notification Service"]

B --> C["Create Notification Record"]

C --> D["Persist Notification"]

D --> E["Start Async Processing"]

E --> F["SMTP Mail Server"]

F --> G{"Email Sent?"}

G -- No --> H["Retry with Exponential Backoff"]

H --> F

G -- Yes --> I["Update Notification Status"]

I --> J["✅ Notification Delivered"]
```

### Workflow Summary

- Business service triggers notification.
- Notification is persisted.
- Email processing occurs asynchronously.
- Failed deliveries are retried automatically.
- Delivery status is tracked.

---

# ❌ Booking Cancellation Workflow

Users can cancel bookings based on business rules and cancellation policies.

```mermaid
flowchart LR

A["👤 User"]

--> B["📅 Booking Service"]

B --> C["Validate Cancellation Request"]

C --> D{"Cancellation Allowed?"}

D -- No --> E["❌ Cancellation Rejected"]

D -- Yes --> F["Cancel Booking"]

F --> G["💳 Payment Service"]

G --> H["Process Refund"]

H --> I["📧 Notification Service"]

I --> J["Send Cancellation Email"]

J --> K["✅ Cancellation Completed"]
```

### Workflow Summary

- Booking Service validates cancellation eligibility.
- Booking status is updated.
- Refund is initiated if applicable.
- Customer receives cancellation notification.

---

# 💰 Refund Workflow

Refund processing is handled independently by the Payment Service.

```mermaid
flowchart LR

A["Booking Cancelled"]

--> B["💳 Payment Service"]

B --> C["Validate Refund Eligibility"]

C --> D{"Eligible?"}

D -- No --> E["Refund Rejected"]

D -- Yes --> F["Initiate Razorpay Refund"]

F --> G["Update Payment Record"]

G --> H["Generate Refund Receipt"]

H --> I["📧 Notification Service"]

I --> J["Notify Customer"]

J --> K["✅ Refund Completed"]
```

### Workflow Summary

- Payment Service validates refund rules.
- Razorpay refund is initiated.
- Payment history is updated.
- Refund notification is delivered.

---

# 🏢 Owner Management Workflow

Property owners can monitor and manage their business through the Owner Service.

```mermaid
flowchart LR

A["🏢 Owner"]

--> B["🌐 API Gateway"]

B --> C["🏢 Owner Service"]

C --> D["Retrieve Owner Properties"]

D --> E["Retrieve Booking Statistics"]

E --> F["Calculate Revenue Summary"]

F --> G["Calculate Occupancy Rate"]

G --> H["Generate Dashboard"]

H --> I["✅ Dashboard Response"]
```

### Workflow Summary

- Owner accesses dashboard.
- Owner Service aggregates business information.
- Revenue and occupancy statistics are calculated.
- Dashboard response is returned.

---

# 🌐 Platform Collaboration Overview

The following diagram illustrates how the primary microservices collaborate to deliver business functionality.

```mermaid
flowchart TD

Client["👤 Client"]

Gateway["🌐 API Gateway"]

Auth["🔐 Auth Service"]

User["👤 User Service"]

Owner["🏢 Owner Service"]

Property["🏠 Property Service"]

Booking["📅 Booking Service"]

Payment["💳 Payment Service"]

Notification["📧 Notification Service"]

Client --> Gateway

Gateway --> Auth
Gateway --> User
Gateway --> Owner
Gateway --> Property
Gateway --> Booking
Gateway --> Payment

Auth --> User
Auth --> Owner

Property --> Owner

Booking --> Property
Booking --> User
Booking --> Payment
Booking --> Notification

Payment --> Booking
Payment --> Notification
```

---

# 🌟 Why This Architecture?

StayEase adopts a distributed microservices architecture to achieve scalability, maintainability, and clear business ownership.

### Enterprise Benefits

- ✅ Independent service deployment
- ✅ Database per Service
- ✅ Clear domain boundaries
- ✅ Better scalability
- ✅ Fault isolation
- ✅ Loose coupling
- ✅ Independent technology evolution
- ✅ Easier testing
- ✅ Enterprise-grade maintainability
- ✅ Cloud-native readiness

This architecture enables each microservice to evolve independently while collaborating through well-defined APIs, making StayEase a scalable and production-oriented accommodation booking platform.

---

# 🏛 Enterprise Architecture Decisions

StayEase has been architected using modern software engineering principles to ensure scalability, maintainability, security, and long-term extensibility.

The following sections explain the rationale behind the key architectural decisions adopted throughout the platform.

---

# 🌐 Why Microservices?

StayEase follows a **Microservices Architecture**, where each business capability is implemented as an independent service.

Instead of developing a large monolithic application, responsibilities are separated into specialized services such as Authentication, Property Management, Booking, Payment, and Notification.

### Benefits

- Independent deployment
- Independent scaling
- Better fault isolation
- Easier maintenance
- Clear business ownership
- Faster development cycles
- Technology flexibility
- Cloud-native readiness

---

# 🚪 Why API Gateway?

The **API Gateway** serves as the single entry point for all client requests.

Rather than exposing every microservice directly to external consumers, the gateway centralizes request routing and provides a unified interface.

```mermaid
flowchart LR

Client["👤 Client"]

Gateway["🌐 API Gateway"]

Auth["🔐 Auth"]

User["👤 User"]

Property["🏠 Property"]

Booking["📅 Booking"]

Payment["💳 Payment"]

Notification["📧 Notification"]

Client --> Gateway

Gateway --> Auth
Gateway --> User
Gateway --> Property
Gateway --> Booking
Gateway --> Payment
Gateway --> Notification
```

### Benefits

- Single entry point
- Simplified client integration
- Centralized routing
- Security enforcement
- Request forwarding
- Future rate limiting
- Future API versioning

---

# 🗄 Why Database per Service?

Each microservice owns its own dedicated database.

No service accesses another service's database directly.

```mermaid
flowchart LR

Auth["Auth Service"] --> AuthDB[(Auth DB)]

User["User Service"] --> UserDB[(User DB)]

Owner["Owner Service"] --> OwnerDB[(Owner DB)]

Property["Property Service"] --> PropertyDB[(Property DB)]

Booking["Booking Service"] --> BookingDB[(Booking DB)]

Payment["Payment Service"] --> PaymentDB[(Payment DB)]

Notification["Notification Service"] --> NotificationDB[(Notification DB)]
```

### Benefits

- Loose coupling
- Independent schema evolution
- Better fault isolation
- Independent backups
- Easier scaling
- Better security boundaries

---

# 🔐 Why JWT Authentication?

Authentication is centralized within the Authentication Service.

Once a user successfully logs in, a signed JWT Access Token and Refresh Token are issued.

Business services trust the JWT instead of storing user sessions.

```mermaid
sequenceDiagram

participant User

participant Gateway

participant Auth

participant Booking

User->>Gateway: Login

Gateway->>Auth: Authenticate

Auth-->>Gateway: JWT + Refresh Token

Gateway-->>User: Tokens

User->>Gateway: Booking Request (JWT)

Gateway->>Booking: Forward Request

Booking->>Booking: Validate JWT

Booking-->>User: Authorized Response
```

### Benefits

- Stateless authentication
- Horizontal scalability
- Reduced database lookups
- Secure authorization
- Better performance

---

# 📡 Why OpenFeign?

Microservices communicate using **OpenFeign Clients**.

Each service exposes REST APIs while other services consume them through declarative interfaces.

```mermaid
flowchart LR

Booking --> Property

Booking --> Payment

Booking --> Notification

Property --> Owner

Auth --> User

Auth --> Owner
```

### Benefits

- Simplified REST communication
- Strong typing
- Cleaner code
- Better maintainability
- Easy integration with Resilience4j

---

# 💳 Why a Dedicated Payment Service?

Payment processing is isolated from booking management.

This separation keeps financial transactions independent from booking logic.

```mermaid
flowchart LR

Booking["📅 Booking Service"]

Payment["💳 Payment Service"]

Razorpay["💰 Razorpay"]

Booking --> Payment

Payment --> Razorpay

Razorpay --> Payment

Payment --> Booking
```

### Responsibilities

- Create payment orders
- Verify payment signatures
- Process refunds
- Track payment history
- Generate receipts

---

# 📧 Why a Dedicated Notification Service?

Notification delivery is separated from core business operations.

This prevents email sending from delaying user-facing operations.

```mermaid
flowchart LR

Business["Business Service"]

Notification["📧 Notification Service"]

SMTP["SMTP Server"]

Business --> Notification

Notification --> SMTP

SMTP --> Notification

Notification --> Business
```

### Responsibilities

- Email notifications
- Retry mechanism
- Exponential backoff
- Delivery tracking
- Duplicate prevention

---

# 🏗 Why Layered Architecture?

Every microservice follows a consistent layered architecture.

```mermaid
flowchart TD

Controller["🌐 Controller"]

Service["⚙️ Service"]

Repository["🗄 Repository"]

Database[("💾 Database")]

Controller --> Service

Service --> Repository

Repository --> Database
```

### Benefits

- Clear separation of concerns
- Easier testing
- Better maintainability
- Improved readability
- Reduced code duplication

---

# 🔄 Why Transaction Management?

Business operations that modify multiple entities are executed within transactional boundaries.

Examples include:

- Booking creation
- Payment verification
- Booking cancellation
- Refund processing

### Benefits

- Atomic operations
- Data consistency
- Rollback support
- Improved reliability

---

# 🛡 Security Principles

Security has been incorporated into every layer of the platform.

Implemented security measures include:

- JWT Authentication
- Refresh Tokens
- BCrypt Password Encryption
- Email Verification
- Role-Based Access Control (RBAC)
- Input Validation
- Global Exception Handling
- Secure Payment Verification
- Protected Internal APIs

Future enhancements include:

- OAuth2
- Multi-Factor Authentication (MFA)
- API Rate Limiting
- Redis Token Blacklisting

---

# 🚀 Production Readiness

StayEase has been designed with production deployment in mind.

Current implementation includes:

- Layered Architecture
- Environment-Based Configuration
- Global Exception Handling
- Centralized Logging
- DTO-Based API Contracts
- Bean Validation
- Service Isolation
- Database per Service

Planned enhancements include:

- Apache Kafka
- Docker
- Kubernetes
- Prometheus
- Grafana
- OpenTelemetry
- Zipkin
- ELK / Loki
- GitHub Actions
- Cloud Deployment

---

# 🌟 Architectural Principles

StayEase follows several enterprise software engineering principles:

- SOLID Principles
- Separation of Concerns
- Single Responsibility Principle
- Domain-Driven Design (DDD)
- Loose Coupling
- High Cohesion
- Stateless Services
- Fail-Fast Validation
- API-First Design
- Secure by Default
- Cloud-Native Ready Architecture

These principles ensure that the platform remains scalable, maintainable, and adaptable as new business requirements emerge.

---

# 📂 Repository Structure

The StayEase repository is organized to separate source code, architecture documentation, developer guides, reusable assets, and API collections. This structure improves maintainability, onboarding, and scalability as the platform evolves.

```text
StayEase/
│
├── README.md                           # Project overview and documentation
├── LICENSE                             # MIT License
├── .gitignore                          # Git ignore rules
│
├── architecture/                       # Enterprise architecture documentation
│   ├── README.md
│   ├── 01-project-overview.md
│   ├── 02-system-architecture.md
│   ├── 03-er-diagram.md
│   ├── 04-class-diagram.md
│   ├── 05-service-dependency.md
│   ├── 06-security-architecture.md
│   ├── 07-feign-communication.md
│   ├── 08-booking-service-design.md
│   ├── 09-payment-service-design.md
│   ├── 10-notification-service-design.md
│   ├── 11-deployment-architecture.md
│   ├── 12-distributed-transactions.md
│   └── 13-future-roadmap.md
│
├── docs/                               # Developer documentation
│   ├── getting-started.md
│   ├── authentication-workflow.md
│   ├── booking-workflow.md
│   ├── payment-workflow.md
│   ├── notification-workflow.md
│   ├── troubleshooting.md
│   ├── api-overview.md
│   └── roadmap.md
│
├── assets/                             # Architecture diagrams and images
│   ├── architecture/
│   ├── workflows/
│   ├── database/
│   └── screenshots/
│
├── postman/                            # API collections
    └── StayEase.postman_collection.json

```

## 📁 Folder Overview

| Folder | Description |
|---------|-------------|
| **architecture/** | Contains enterprise architecture documents, design decisions, diagrams, and technical references. |
| **docs/** | Developer documentation including setup guides, workflows, troubleshooting, and API usage. |
| **assets/** | Stores architecture diagrams, workflow diagrams, ER diagrams, screenshots, and other visual resources. |
| **postman/** | Contains Postman collections for testing and exploring the platform APIs. |
| **services/** | Contains the individual microservice repositories that together form the StayEase platform. |

The repository structure is designed to keep business logic, documentation, diagrams, and supporting resources well organized, making the project easier to understand, maintain, and extend.

---

# 🔗 Service Repositories

StayEase follows a distributed microservices architecture where each business domain is developed, versioned, and deployed independently.

Each microservice maintains its own source code repository, allowing independent development, testing, deployment, and future scalability.

| Service | Responsibility | Technology | Status |
|----------|----------------|------------|--------|
| 🌐 API Gateway | API routing, request forwarding, centralized entry point | Spring Cloud Gateway | ✅ Completed |
| 🔐 Auth Service | Authentication, JWT, Refresh Tokens, Email Verification | Spring Boot, Spring Security | ✅ Completed |
| 👤 User Service | User profile management, wishlist, booking history | Spring Boot, Spring Data JPA | ✅ Completed |
| 🏢 Owner Service | Owner dashboard, property ownership, revenue analytics | Spring Boot | ✅ Completed |
| 🏠 Property Service | Property listings, rooms, amenities, search, reviews | Spring Boot | ✅ Completed |
| 📅 Booking Service | Booking lifecycle, availability calculation, cancellations | Spring Boot | ✅ Completed |
| 💳 Payment Service | Razorpay integration, payment verification, refunds | Spring Boot | ✅ Completed |
| 📧 Notification Service | Email notifications, retry mechanism, delivery tracking | Spring Boot | ✅ Completed |

## 📦 Repository Organization

Each service follows the same enterprise project structure to ensure consistency across the platform.

```text
service-name/
│
├── src/
├── docs/
├── README.md
├── build.gradle
├── gradlew
├── gradlew.bat
├── settings.gradle
├── .gitignore
└── LICENSE
```

## 🎯 Why Separate Repositories?

StayEase adopts a multi-repository (multi-repo) strategy to align with enterprise software development practices.

### Benefits

- Independent development for each service
- Independent release cycles
- Independent deployments
- Better ownership of business domains
- Cleaner Git history
- Easier team collaboration
- Service-specific CI/CD pipelines
- Independent versioning
- Improved scalability and maintainability

This repository serves as the central documentation hub, while each microservice repository contains the implementation, configuration, and service-specific documentation.

---

# 🚀 Getting Started

This guide explains how to set up and run the StayEase platform in a local development environment.

## 📋 Prerequisites

Ensure the following software is installed before running the project.

| Software | Version |
|----------|---------|
| Java | 21 or later |
| Gradle | 8.x or later |
| MySQL | 8.0 or later |
| Git | Latest |
| IntelliJ IDEA / VS Code | Latest |
| Postman | Latest (Optional) |

---

## 📥 Clone the Repositories

Clone the required StayEase repositories from GitHub.

```bash
git clone https://github.com/PSaiRam32/stayease-api-gateway
git clone https://github.com/PSaiRam32/stayease-auth-service
git clone https://github.com/PSaiRam32/stayease-user-service
git clone https://github.com/PSaiRam32/stayease-owner-service
git clone https://github.com/PSaiRam32/stayease-property-service
git clone https://github.com/PSaiRam32/stayease-booking-service
git clone https://github.com/PSaiRam32/stayease-payment-service
git clone https://github.com/PSaiRam32/stayease-notification-service
```

---

## 🗄 Database Setup

Create a separate MySQL database for each microservice.

| Service | Database |
|----------|----------|
| Auth Service | `stayease_auth_db` |
| User Service | `stayease_user_db` |
| Owner Service | `stayease_owner_db` |
| Property Service | `stayease_property_db` |
| Booking Service | `stayease_booking_db` |
| Payment Service | `stayease_payment_db` |
| Notification Service | `stayease_notification_db` |

---

## ⚙️ Configure Environment

Update the `application.yml` (or profile-specific configuration) in each service with your local settings.

Typical configuration includes:

- MySQL URL
- Database username
- Database password
- SMTP credentials
- Razorpay API credentials
- JWT secret
- Service ports

---

## ▶️ Start the Services

Start the services in the following order:

1. Auth Service
2. User Service
3. Owner Service
4. Property Service
5. Booking Service
6. Payment Service
7. Notification Service
8. API Gateway

Verify that each service starts successfully before launching the next.

---

## 🌐 Access the APIs

After all services are running, access the platform through the API Gateway.

Example:

```
http://localhost:8080
```

Use the API Gateway as the single entry point for all client requests.

---

## 🧪 Verify the Setup

After starting all services:

- Confirm each service is running without startup errors.
- Verify database connections.
- Open the Swagger UI for each service.
- Register a user or owner.
- Verify email confirmation.
- Log in and obtain JWT tokens.
- Search for properties.
- Create a booking.
- Complete a payment.
- Verify notification delivery.

If all of the above work successfully, the StayEase platform is ready for development and testing.

---

# 📮 API Documentation

StayEase follows an API-first approach where every microservice exposes RESTful APIs documented using **Swagger / OpenAPI**.

Each service provides an interactive Swagger UI that allows developers to:

- Explore available endpoints
- View request and response models
- Test APIs directly from the browser
- Understand validation rules
- Review HTTP status codes

## 📚 Swagger Endpoints

| Service | Default Port | Swagger UI |
|----------|-------------:|------------|
| API Gateway | 8000 | Gateway routes client requests (Swagger typically hosted by services) |
| Auth Service | 8081 | `http://localhost:8081/swagger-ui/index.html` |
| User Service | 8082 | `http://localhost:8082/swagger-ui/index.html` |
| Owner Service | 8083 | `http://localhost:8083/swagger-ui/index.html` |
| Property Service | 8084 | `http://localhost:8084/swagger-ui/index.html` |
| Booking Service | 8085 | `http://localhost:8085/swagger-ui/index.html` |
| Payment Service | 8086 | `http://localhost:8086/swagger-ui/index.html` |
| Notification Service | 8087 | `http://localhost:8087/swagger-ui/index.html` |

## API Design Principles

StayEase APIs follow consistent RESTful design practices:

- Resource-oriented endpoint naming
- Standard HTTP methods
- DTO-based request and response models
- Consistent HTTP status codes
- Bean Validation
- Global Exception Handling
- JWT-secured endpoints
- Role-Based Access Control (RBAC)

This consistency simplifies client integration and improves maintainability across all microservices.

---

# 🤝 Contributing

Contributions, suggestions, and constructive feedback are always welcome.

If you would like to contribute:

1. Fork the repository.
2. Create a feature branch.
3. Follow the existing coding standards and project structure.
4. Commit your changes with meaningful commit messages.
5. Push your branch to your fork.
6. Open a Pull Request describing your changes.

## Development Guidelines

- Follow SOLID principles.
- Maintain layered architecture.
- Keep services loosely coupled.
- Write clean and readable code.
- Validate inputs using Jakarta Bean Validation.
- Handle exceptions through Global Exception Handlers.
- Keep business logic inside the service layer.
- Update documentation whenever new features are introduced.

Thank you for helping improve StayEase.

---

# 📜 License

This project is licensed under the **MIT License**.

You are free to use, modify, and distribute this software in accordance with the terms of the MIT License.

See the `LICENSE` file for the complete license text.

---

# 👨‍💻 Author

**Sai Ram Paidipati**

Java Backend Developer 

### Connect with me

- GitHub: https://github.com/PSaiRam32
- LinkedIn: https://www.linkedin.com/in/sairam-paidipati/

If you found this project helpful, consider giving the repository a ⭐.

---
