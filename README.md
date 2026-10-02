# Salesforce Field Service Notebook
A practical learning repository focused on Salesforce Field Service, field service operations, and technical English.

## Professional Context

I currently work in a Maintenance Planning and Control (PCM) environment where Salesforce Field Service is used to support service operations.

My professional experience gives me practical exposure to field service and maintenance processes, while this repository focuses on deepening my technical knowledge of Salesforce Field Service and developing my technical English.

## About

This repository documents my learning journey as I deepen my knowledge of Salesforce Field Service, connecting the platform's concepts with real-world maintenance and field service processes.

The goal is to move beyond being a platform user and develop a deeper understanding of how Salesforce Field Service supports:

- Field service operations
- Work management
- Service scheduling
- Dispatching
- Field resources
- Assets and maintenance
- Inventory and parts
- Automation
- Reporting and data

The repository also serves as a way to develop my technical English vocabulary and practice explaining Salesforce concepts in English.

---

## Learning Goals

- Understand Salesforce Field Service concepts and architecture
- Improve my knowledge of the Salesforce data model
- Understand how field service operations are represented in Salesforce
- Learn scheduling and dispatching concepts
- Explore assets, maintenance, inventory, and mobile operations
- Develop practical Salesforce knowledge through hands-on exercises
- Build Salesforce-related projects and documentation
- Improve technical English for international professional environments
- Prepare for future Salesforce and Field Service-related interviews

---

## Current Focus

**Field Service Operations**

Currently preparing to explore:

- Field service operations
- Scheduling
- Dispatching
- Service resources
- Service appointments
- Field service terminology

---

## Trailhead Learning Path

| Module / Trail | Status |
|---|---|
| Field Service Basics | ✅ Completed |
| Field Service: Optimize Operations in the Field | ⏳ Next |
| Field Service Dispatcher | ⏳ Planned |
| Agentforce for Field Service | ⏳ Planned |

> This repository is continuously updated as I progress through my Salesforce Field Service learning journey.

---

## Roadmap

### Phase 1 — Fundamentals

- [x] Field Service basics
- [ ] Core Field Service objects
- [ ] Service Territories
- [ ] Service Resources
- [ ] Work Orders
- [ ] Service Appointments

### Phase 2 — Field Operations

- [ ] Scheduling
- [ ] Dispatching
- [ ] Dispatcher Console
- [ ] Mobile Field Service
- [ ] Travel and operating hours

### Phase 3 — Maintenance

- [ ] Assets
- [ ] Asset hierarchy
- [ ] Maintenance Plans
- [ ] Preventive Maintenance
- [ ] Work management

### Phase 4 — Advanced Topics

- [ ] Inventory and parts
- [ ] Automation and Flow
- [ ] Reports and dashboards
- [ ] Data model
- [ ] Integrations

### Phase 5 — Practical Projects

- [ ] Field Service process simulation
- [ ] Scheduling scenario
- [ ] Maintenance workflow
- [ ] Automation project
- [ ] End-to-end Field Service project

---

## Learning Approach

My learning process combines four areas:

### 1. Salesforce

Learning the platform and its Field Service capabilities through Trailhead and hands-on practice.

### 2. Real-world experience

Connecting Salesforce concepts with processes I encounter in my professional experience in PCM and maintenance operations.

### 3. Technical English

Studying Salesforce documentation and Trailhead content in English while building a technical vocabulary focused on Field Service.

### 4. Practical Projects

Applying what I learn through exercises, documentation, simulations, and future Salesforce-related projects.

---

## Repository Structure

```text
salesforce-field-service-notebook/
│
├── README.md
│
├── 01-fundamentals/          (Phase 1)
│   └── field-service-basics.md
│
├── 02-field-operations/      (Phase 2: scheduling, dispatching, mobile)
│
├── 03-maintenance/           (Phase 3: assets, maintenance, preventive maintenance)
│
├── 04-advanced/              (Phase 4: inventory, automation, reports, data model, integrations)
│
├── 05-projects/              (Phase 5)
│
├── vocabulary/
│
├── interview/
│
└── learning-log/
```
# Salesforce Field Service Basics

## Overview
Field Service is a Salesforce product to manage maintenance operations, where the planner views the skills of service resources, service territories, service territory members and operating hours of the service territory and service resource, and also the scheduling for resources.
This section documents the fundamental concepts I learned while completing the Salesforce Trailhead Field Service Basics module.
My goal is to understand not only how Salesforce Field Service is used, but also how its concepts relate to real-world maintenance and field service operations.

## Key Concepts

### Users
A User is an individual account that allows a person to access Salesforce.
In the Field Service context, users can have different responsibilities, such as field technicians, dispatchers, service managers, planners, or agents.
A user can also be associated with a Service Resource when the person needs to be managed as a resource for field service operations.

### Service Resource
A Service Resource represents a person, crew, or other resource that can be scheduled to perform field service work.
For example, a field technician can be represented as a Service Resource and associated with a Salesforce User.
Service Resources can be related to skills, service territories, and availability, which helps Salesforce determine whether a resource is suitable for a specific service.

### Service Territory
A Service Territory represents a geographical or operational area where field service work is performed.
Service Territories help organizations organize their field service operations based on location or operational coverage.
A Service Resource can be associated with one or more Service Territories depending on the organization's configuration and operational requirements.

### Service Territory Members
A Service Territory Member represents the association between a Service Resource and a Service Territory.
This relationship defines which service territory a resource is assigned to or can operate in.
For example, a field technician can be represented as a Service Resource and associated with the Campinas Service Territory through a Service Territory Member.

### Operating Hours
Operating Hours define when a service operation, territory, or resource is available to perform field service work.
They help determine when service appointments can be scheduled based on the organization's operating schedule.
Operating Hours can therefore be an important factor when determining whether a service can be performed at a specific time.

### Skills
Skills represent the abilities or qualifications required to perform specific types of field service work.
A Service Resource can have one or more skills, and these skills can be used when determining whether the resource is qualified for a specific service appointment.

## How These Concepts Connect
The concepts introduced in Field Service are connected to help organizations manage field service resources and determine who can perform a specific service.

A simplified relationship can be represented as:

```text
Service Territory
        ↑
        │
Service Territory Member
        │
        ↓
Service Resource
        │
        └── Service Resource Skill ──→ Skill

Operating Hours → linked to the Service Territory and to the Service Territory Member
Availability    → result of Operating Hours, absences, and existing appointments
```

A Service Resource can be associated with a Salesforce User.

These relationships provide information that can be used when scheduling and assigning field service work.

## Connection With My PCM Experience
My current role in Maintenance Planning and Control (PCM) involves planning and coordinating external technicians.
Because of this experience, I was able to relate Salesforce Field Service concepts such as Service Resources, Service Territories, Service Territory Members, Skills, and Operating Hours to real-world field service operations.
For example, when planning an external technician, it is necessary to consider factors such as the technician's area of operation, availability, working hours, and technical capabilities.
Understanding how Salesforce represents these concepts helped me connect my existing operational knowledge with the platform's data model and field service processes.

## Technical English

| Term | Português | Example |
|---|---|---|
| User | Usuário | The user can access Salesforce based on their permissions. |
| Service Resource | Recurso de serviço | The technician is represented as a Service Resource. |
| Service Territory | Território de serviço | The technician is assigned to a Service Territory. |
| Service Territory Member | Relação entre recurso e território | The Service Territory Member connects the Service Resource to the Service Territory. |
| Operating Hours | Horário de funcionamento/operação | The service must be scheduled within the operating hours. |
| Skill | Habilidade/qualificação | The technician has the required skill for the job. |
| Availability | Disponibilidade | The technician's availability must be considered when scheduling the appointment. |

## Key Takeaways
- A Salesforce User represents an individual account that can access the platform.
- A Service Resource represents a person, crew, or other resource that can be scheduled for field service work.
- A Service Territory represents a geographical or operational area where field service work is performed.
- A Service Territory Member represents the association between a Service Resource and a Service Territory.
- Skills represent the abilities or qualifications required to perform specific field service work.
- Operating Hours help define when field service operations can be performed.
- These concepts work together to support field service scheduling and resource management.
