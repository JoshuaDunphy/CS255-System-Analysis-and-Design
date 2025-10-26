# CS 255 Portfolio – DriverPass System Analysis & Design

---

## Project Summary

**DriverPass** is a startup founded by **Liam**, with support from his IT officer **Ian**, focused on reducing the high DMV test failure rate (over 65%) through better driver education. The client requested a **web-based learning and scheduling platform** that includes:

- Online practice exams with instant feedback
- Progress tracking dashboards
- On-the-road training scheduling with certified instructors
- Secure payment processing
- Admin tools for content management and user monitoring

This project involved two key deliverables:
- **Project One**: Business Requirements Document
- **Project Two**: System Design Document (including UML diagrams)

---

## What I Did Particularly Well

I excelled in **creating clear, accurate UML diagrams** that directly reflected the client’s needs. The **Use Case Diagram** effectively captured all user roles and interactions, while the **Activity Diagram** for *Take Practice Exam* provided a detailed, logical flow that supports student learning. My **Class Diagram** was well-structured with proper relationships (e.g., `Student` to `Schedule`, `Student` to `Course` via enrollment), demonstrating strong object-oriented design principles.

---

## One Area I’d Revise

If I could revise one part, I would improve the **Sequence Diagram** by including **error handling paths** (e.g., invalid login, insufficient funds, payment failure). While the current version clearly shows the happy path, adding alternative flows would make the design more robust and better prepare developers for real-world scenarios.

---

## Interpreting User Needs

I interpreted the client’s needs by thoroughly reviewing the **DriverPass Interview Transcript** and **Business Requirements Document**. Key insights included:

- Liam’s emphasis on **practice exams with feedback** → Led to detailed activity and sequence diagrams
- Ian’s focus on **cloud backup and security** → Influenced technical requirements (e.g., encrypted storage, SSL/TLS)
- Need for **progress tracking** → Added `progressScore` attribute in `Student` class

**User needs are the foundation of good design.** A system that doesn’t solve real problems—even if technically perfect—will fail. By prioritizing usability, accessibility, and security, I ensured the system supports students, instructors, and admins effectively.

---

## My Approach to Software Design

I follow a **user-centered, structured, and iterative** approach:

1. **Gather & Clarify** – Conduct interviews, analyze transcripts, and document requirements
2. **Model Behavior** – Use **UML diagrams** (Use Case, Activity, Sequence, Class) to visualize functionality and structure
3. **Validate** – Cross-check designs against client goals and constraints (budget, timeline)
4. **Simplify & Scale** – Focus on core features first, design modularly for future growth

In the future, I’ll continue using:
- **Lucidchart** for UML modeling
- **GitHub** for version control and collaboration
- **Agile principles** to refine designs based on feedback

---

## Submitted Artifacts

| File | Description |
|------|-----------|
| [`CS255_DriverPass_BusinessRequirements.docx`](CS255_DriverPass_BusinessRequirements.docx) | Project One – Full requirements gathering and documentation |
| [`CS255_DriverPass_SystemDesignDocument.docx`](CS255_DriverPass_SystemDesignDocument.docx) | Project Two – UML diagrams and technical specifications |

---

> *“Great systems begin with great understanding.”*  
> This project reinforced the importance of listening to users, modeling clearly, and designing for both today and tomorrow.

---