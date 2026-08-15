# Hi, I'm Yash Lodam 👋

### Java Full Stack Developer · Spring Boot · React.js · PostgreSQL · AI Engineering

I build full-stack applications and backend systems with Java and Spring Boot, create
modern interfaces with React.js, and explore AI engineering with Spring AI, RAG, vector
search, and LLM tool calling.

My focus is on building software with clean architecture, secure APIs, reliable
persistence, and maintainable code — while continuously expanding toward microservices,
system design, and AI-powered applications.

<br/>

![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=spring-boot&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring%20Security-6DB33F?style=flat-square&logo=spring-security&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Spring AI](https://img.shields.io/badge/Spring%20AI-6DB33F?style=flat-square&logo=spring&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

<br/>

## 👨‍💻 About Me

I'm a Computer Engineering student at SPPU, graduating in 2027, with a primary focus on
Java backend and full-stack development.

I enjoy building applications from the ground up — designing APIs, modeling databases,
implementing authentication and business logic, connecting frontend and backend systems,
and integrating AI capabilities where they provide real value.

**What I'm focused on**

- ☕ Java & Spring Boot backend development
- 🔐 Spring Security, JWT & OTP authentication
- 🌐 REST API & full-stack application development
- ⚛️ React.js frontend development
- 🗄️ PostgreSQL, MySQL & MariaDB
- 🤖 Spring AI, RAG & LLM integrations
- 🧩 Microservices & distributed systems
- 🏗️ System design & scalable backend architecture
- 🧠 Data Structures & Algorithms

<br/>

## 🛠️ Tech Stack

**Languages**
`Java` `JavaScript` `C++` `SQL`

**Backend**
`Spring Boot` `Spring MVC` `Spring Data JPA` `Hibernate`
`Spring Security` `JWT` `OTP` `REST APIs` `Maven`

**Frontend**
`React.js` `JavaScript` `HTML5` `CSS3`
`Tailwind CSS` `Bootstrap` `jQuery`

**Databases**
`PostgreSQL` `MySQL` `MariaDB`

**AI / GenAI**
`Spring AI` `Google Gemini` `RAG`
`Vector Stores` `Embeddings` `Chat Memory` `Tool Calling`

**Tools**
`Git` `GitHub` `Docker` `Postman` `VS Code` `Eclipse / STS`

<br/>

## 🚀 Featured Projects

### 🛒 ShopSphere — Multi-Vendor E-Commerce Platform

A full-stack multi-vendor e-commerce platform designed around separate customer and
seller workflows, with a layered Spring Boot backend and React frontend.

**Key Engineering Areas**

- Customer and seller authentication
- JWT-based authorization
- OTP verification
- Seller and business management
- Product and category management
- Product search and filtering
- Price, size, color and category filtering
- Cart and cart-item management
- Order and order-item processing
- Seller-specific order processing
- Razorpay payment integration
- Cash-on-delivery workflow
- PostgreSQL persistence

**Architecture**

```text
┌──────────────────────┐
│      React.js        │
│  Redux · Tailwind    │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│      REST APIs       │
│     Spring Boot      │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│    Service Layer     │
│   Business Logic     │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│  Repository / JPA    │
│      Hibernate       │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│     PostgreSQL       │
└──────────────────────┘
```

**Stack:** `Java` · `Spring Boot` · `Spring Security` · `JWT` · `React` · `Redux Toolkit` · `PostgreSQL` · `JPA/Hibernate`

---

### 🤖 AI HelpDesk — AI-Powered Support System

A full-stack customer support platform where an AI assistant can interact with
application data through Spring AI tool calling. The goal is to move beyond a simple
chatbot and allow the model to perform meaningful application operations through
controlled backend tools.

**Key Engineering Areas**

- Conversational AI support
- Persistent conversation memory
- Ticket creation through AI tools
- Ticket retrieval
- Ticket updates
- Database-aware AI interactions
- Spring AI tool calling
- Google Gemini integration
- React chat interface
- PostgreSQL persistence

**Architecture**

```text
┌──────────────────────┐
│    React Chat UI     │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│     Spring Boot      │
│      ChatClient      │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│      Spring AI       │
│   Chat Memory + AI   │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│    Google Gemini     │
└──────────┬───────────┘
           │
       Tool Calling
           │
           ▼
┌──────────────────────┐
│    Ticket Service    │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│     PostgreSQL       │
└──────────────────────┘
```

**Stack:** `Java` · `Spring Boot` · `Spring AI` · `Google Gemini` · `React` · `Tailwind CSS` · `PostgreSQL`

---

### 🧠 Spring RAG — Retrieval-Augmented Generation

A Spring Boot application exploring how Retrieval-Augmented Generation can ground LLM
responses in application-specific knowledge. Instead of relying only on the model's
internal knowledge, the system retrieves relevant information from a vector store and
provides that context to the LLM.

**Key Concepts**

- Document ingestion
- Embedding generation
- Vector storage
- Similarity search
- RAG pipelines
- Chat memory
- Conversation IDs
- `ChatClient`
- `MessageChatMemoryAdvisor`
- `QuestionAnswerAdvisor`
- VectorStore integration
- Dockerized MariaDB vector infrastructure

**Architecture**

```text
              User
                │
                ▼
        ┌───────────────┐
        │  Spring Boot  │
        └───────┬───────┘
                │
                ▼
          ┌───────────┐
          │ ChatClient│
          └─────┬─────┘
                │
                ▼
          ┌───────────┐
          │ RAG Layer │
          └─────┬─────┘
                │
                ▼
        ┌───────────────┐
        │ Vector Store  │
        │    MariaDB    │
        └───────┬───────┘
                │
         Similarity Search
                │
                ▼
        Relevant Documents
                │
                ▼
             LLM
                │
                ▼
            Response
```

**Stack:** `Spring Boot` · `Spring AI` · `Google Gemini` · `RAG` · `MariaDB Vector Store` · `Docker`

---

### 💼 Velora — AI-Powered Job Platform

A full-stack job platform focused on job discovery, recruiter workflows, candidate
profiles, and modern user experience.

**Key Areas**

- Job discovery and search
- Location-based search
- Candidate workflows
- Recruiter workflows
- Profile management
- Resume-oriented features
- Modern responsive interface
- Component-based React architecture
- AI-powered feature exploration

**Frontend Architecture**

```text
React
 │
 ├── Mantine UI
 ├── Tailwind CSS
 ├── Framer Motion
 └── React Router
 │
 ▼
REST APIs
 │
 ▼
Spring Boot
 │
 ▼
PostgreSQL
```

**Stack:** `React` · `Tailwind CSS` · `Mantine` · `Framer Motion` · `Java` · `Spring Boot` · `PostgreSQL`

<br/>

## 🏗️ Engineering Approach

I try to approach projects as software systems, not just collections of features.

**Backend**

```text
Controller
    ↓
Service
    ↓
Repository
    ↓
Database
```

**Core principles**

- Separation of concerns
- Layered architecture
- RESTful API design
- Secure authentication and authorization
- Database relationship modeling
- Transaction management
- Centralized exception handling
- Validation
- Reusable components
- Maintainable code
- Meaningful naming
- Version control with Git

As I progress, I'm extending this foundation toward:

```text
Monolith
   ↓
Modular Architecture
   ↓
Microservices
   ↓
Distributed Systems
   ↓
Scalable Architecture
```

<br/>

## 🤖 AI Engineering

My interest in AI is focused on integrating AI into real software systems, rather than
treating an LLM as a standalone chatbot. I'm currently working with concepts including:

- Retrieval-Augmented Generation
- Vector search
- Embeddings
- Conversational memory
- LLM tool calling
- AI-assisted application workflows
- Spring AI
- Google Gemini
- AI agents
- AI-powered backend architecture

The direction I'm exploring:

```text
LLM
 ↓
Context
 ↓
Retrieval
 ↓
Tools
 ↓
Application Data
 ↓
Business Logic
 ↓
Useful Software
```

<br/>

## 📚 Currently Learning

**☕ Java & Spring**
- Advanced Java
- Spring Boot
- Spring Security
- JPA & Hibernate
- Transactions
- Validation
- Microservices
- Production-oriented backend development

**🏗️ System Design**
- Scalability
- Load balancing
- Caching
- API gateways
- Service discovery
- Message queues
- Distributed systems
- Fault tolerance
- Database design
- Observability

**🤖 AI Engineering**
- Advanced RAG architectures
- AI agents
- Tool-based AI systems
- AI application architecture
- LLM integration patterns

<br/>

## 🧠 Problem Solving

I practice Data Structures & Algorithms in Java to strengthen problem-solving and
algorithmic thinking.

Current areas include:
`Arrays` · `Strings` · `Hashing` · `Searching` · `Sorting` · `Linked Lists` · `Stacks` · `Queues` · `Trees` · `Graphs` · `Dynamic Programming`

**LeetCode:** 57+ problems solved · 68%+ acceptance rate · 20-day maximum streak

<br/>

## 🎓 Education

**B.E. Computer Engineering**
Savitribai Phule Pune University (SPPU)
Late G. N. Sapkal College of Engineering, Nashik
Expected Graduation: 2027

<br/>

## 🏆 Certifications

- Google Cloud Arcade Facilitator
- NPTEL Certification
- Internship Studio Certification

<br/>

## 📊 GitHub Activity

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=yashlodam&show_icons=true&theme=default&hide_border=true&count_private=true" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=yashlodam&layout=compact&hide_border=true" />
</p>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=yashlodam&hide_border=true" />
</p>

<br/>

## 🌐 Connect With Me

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](YOUR_LINKEDIN_URL)
[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=flat-square&logo=vercel&logoColor=white)](YOUR_PORTFOLIO_URL)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:YOUR_EMAIL_ADDRESS)

<br/>

<p align="center"><sub>Open to full-time Java Full Stack Developer roles.</sub></p>
