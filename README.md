# Domain-Driven Design Starter Modelling Process

This process gives you a step-by-step guide for learning and practically applying each aspect of Domain-Driven Design -- from orienting around an organisation's business model to coding a domain model.

Using this process will guide you through each of the essential steps in a designing a software system with the DDD mindset, so you can focus on your business challenges and not be overwhelmed by learning DDD at the same time. 

Once you have been through a few iterations of the process you will have the foundational DDD theory and practical experience to go deeper into DDD. Then you will be able to adapt and improve the process to suit your needs in any context. On a real project you'll constantly be jumping back and forth between all of these steps.

> This process is for beginners. It is not a linear sequence of steps that you should standardise as a best practice. Domain-Driven Design is an evolutionary design process which necessitates continuous iteration on all aspects of knowledge and design.

![DDD Starter Modelling Process](resources/ddd-starter-modelling-process.jpg)

## When to use the DDD Starter Modelling Process?
If you're new to DDD or you're just not sure where to start, this process can reduce you're cognitive and guide you through the process in the following scenarios, and possibly others:

### Kicking Off a Greenfield Project
At the start of a new project the number of things you need to think about can be overwhelming. One or two iterations of this process can help you put the foundations in place.

### Beginning a Brownfield Migration
Before getting to work on moderinising your legacy system, a few iterations of this process can help you to uncover essential information needed to create a vision for your target architecture.

### Kicking Off a Major Program of Work
When starting a new initiative that involves a significant investment across many teams, it is essential to cover the 8 steps in the process. This process can guide you through the first few iterations.

### Explore Your Domain for New Learning Opportunities
Software development is a learning process. You can apply this process at any time to uncover new insights, identify new opportunities, or simply share knowledge around the team.

### Assess Current State of Your Project
This process can be the foundation for assessing how well your current system is aligned to the domain and business model. 

### Re-organising Teams
A loosely-coupled architecture enables teams to work in parallel without being blocked. But a loosely-coupled architecture must be aligned to coupling in the domain. This process will help you to design a software architecture and a team structure aligned with your domain.

### Practicing or Learning DDD
This process is ideal when you are new to DDD and want to practice or you want to teach others the different aspects of modelling a domain. It's important to communicate that this linear process is not a realistic process, it's just a starting point to reduce cognitive load until you are confident with DDD.

## How to Adapt the Process?
On a real project you will find that new information arises and new insights are gained that invalidate the assumptions about the business goals, the domain, or the design of the system. So you will have to re-apply certain steps of the process and possibly in a different order.

There are an infinite number of possibilities for iterating on a design and applying steps in the process. Below are a few examples:

### Start with EventStorming
...

### Start by Assessing IT Landscape
...

### Code Before Confirming Architecture and Team Boundaries
...

### Repeat Steps 2 - 5 Before Moving to 6
...

### Organise Teams Before Designing Contexts
...

### Blending Design and Coding
...

## The Process

### 1. Orient / Align
- business model
- project goals / success metrics
- user needs / user research

#### Why

#### Tools

- business model canvas
- product strategy canvas
- impact mapping
- wardley mapping

#### How to Facilitate

#### Who to Involve
- business stakeholders
- project sponsor
- product management
- C-suite
- technical leadership

### 2. Discover

#### Why
- create shared understanding of business domain across the whole team

#### Tools
- EventStorming
- Domain Storytelling
- User Journey Mapping
- Example Mapping

#### How to Facilitate

#### Who to Involve
- domain experts
- development team
- customer support
- business leadership
- real users
- anyone who has knowledge of the domain 

### 3. Decompose

#### Why
- align software system to business domain so changes are easier 
- minimise coupling 
- reduce cognitive load

#### Tools
- bounded contexts
- design heuristics

#### How to Facilitate

#### Who to Involve
- domain experts
- project managers
- product managers
- software architects
- software engineers

### 4. Integrate / Challenge

Suggestion: rename this to "Challenge The Design with concrete use cases"

#### Why
- design a system of bounded contexts that work together to fulfill business use cases
- reduce coupling
- uncover hidden dependencies
- validate design

#### Tools
- domain message flow modelling
- process-level EventStorming
- sequence diagrams
- strategic domain storytelling
- BPMN


#### How to Facilitate

#### Who to Involve
- software architects
- software engineers
- domain experts
- product managers

### 5. Strategize

#### Why
- identify most important areas to focus on
- analyse existing architecture as IT portfolio
- decide build-vs-buy
- anticipate evolution of system

#### Tools
- Wardley Mapping
- Core Domain Charts
- Purpose Alignment Matrix

#### How to Facilitate

#### Who to Involve
- software architects
- domain experts
- business stakeholders
- product managers
- software engineers

### 6. Design

#### Why
- consider key consequences of the design before building
- explore alternative models
- gain shared agreement on design
- understand how technical limitations will impact business processes

#### Tools
- Bounded Context Canvas
- Aggregate Design Canvas
- Design-level EventStorming
- (((Michael Plod's IOS Standards)))

#### How to Facilitate

#### Who to Involve

### 7. Organise

#### Why

#### Tools

#### How to Facilitate

#### Who to Involve

### 8. Model

#### Why

#### Tools

#### How to Facilitate

#### Who to Involve

## Contributors

Thank you to the following individuals who have all contributed to the DDD Starter Modelling Process:

- [Gien Verschatse](https://twitter.com/selketjah)
- [Kacper Gunia](https://github.com/cakper)
- [James Morcom](https://twitter.com/morcs)
- [Maxime Sanglan-Charlier](https://twitter.com/__MaxS__)
- [Nick Tune](https://github.com/ntcoding)

## Contributions and Feedback

The Domain-Driven Design Starter Modelling Process is freely available for you to use. In addition, your feedback and ideas are welcome to improve the technique or to create alternative versions. 

Feel free to also send us a pull request with your examples or experience reports.

[![CC BY 4.0][cc-by-shield]][cc-by]

This work is licensed under a [Creative Commons Attribution 4.0 International
License][cc-by].

[![CC BY 4.0][cc-by-image]][cc-by]

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg