# Domain-Driven Design Starter Modelling Process

This process gives you a step-by-step guide for learning and practically applying each aspect of Domain-Driven Design - from orienting around an organisation's business model to coding a domain model.

Using this process will guide you through each of the essential steps in designing a software system with the DDD mindset, so you can focus on your business challenges and not be overwhelmed by learning DDD at the same time. 

Once you have been through a few iterations of the process you will have the foundational DDD theory and practical experience to go deeper into DDD. Then you will be able to adapt and improve the process to suit your needs in any context. On a real project you'll often be jumping back and forth between these steps.

> This process is for beginners. It is not a linear sequence of steps that you should standardise as a best practice. Domain-Driven Design is an evolutionary design process which necessitates continuous iteration on all aspects of knowledge and design.

![DDD Starter Modelling Process](resources/ddd-starter-modelling-process.jpg)

## When to use the DDD Starter Modelling Process?
If you're new to DDD or just not sure where to start, this process can reduce your cognitive load. It will guide you through following scenarios, and possibly others:

### Kicking Off a Greenfield Project
At the start of a new project the number of things you need to think about can be overwhelming. One or two iterations of this process can help you put the foundations in place.

### Beginning a Brownfield Migration
Before getting to work on modernising your legacy system, a few iterations of this process can help you to uncover essential information needed to create a vision for your target architecture.

### Kicking Off a Major Program of Work
When starting a new initiative involves a significant investment across many teams, it is essential to cover the 8 steps in the process. This process can guide you through the first few iterations.

### Explore Your Domain for New Learning Opportunities
Software development is a learning process. You can apply the DDD Starter Modelling Process at any time to uncover new insights, identify new opportunities, or simply share knowledge around the team.

### Assess Current State of Your Project
This process can be the foundation for assessing how well your current system is aligned to the domain and business model. 

### Re-organising Teams
A loosely-coupled architecture enables teams to work in parallel without being blocked. A loosely-coupled architecture also must be aligned to coupling in the domain. This process will help you to design a software architecture, and a team structure aligned with your domain.

### Practicing or Learning DDD
This process is ideal when you are new to DDD and want to practice, or you want to teach others the different aspects of modelling a domain. It's important to communicate that this linear process is not a realistic process. It's just a starting point to reduce cognitive load until you are confident with DDD.

## How to Adapt the Process?
This process can be customised in many ways. On a real project, you'll be switching between all 8 steps based on the new insights you gain or need to gain.

Below are a few reasons for deciding when to change the order or switch between steps.

### Start with Collaborative Modelling
If you want to get our whole team collaborating immediately, modelling the domain which they are familiar with might be more comfortable than talking about business models and strategy which they are less comfortable with.

### Start by Assessing IT Landscape
Before looking forward to the business vision and going deep into the domain, it might be better to visualise the existing architecture first. Start with step 5 and map out your strategic portfolio to see what the major constraints you will face are.

### Code Before Confirming Architecture and Team Boundaries
On some projects it makes sense to start by writing code sooner. Perhaps you need to deliver an MVP or the domain is so complex that creating a model in code is necessary before you can consider the architecture.

### Repeat Steps 2 (Discover) - 6 (Organise) Before Moving to 7 (Define)
Before you dive into the definition of individual bounded contexts, it may be beneficial to model the domain multiple times and look for different ways to decompose your system into sub-domains and teams.

### Organise Teams Before Designing Contexts
For a great deal of projects there are organisational constraints that we need to take into account. If this is the case, you should consider identifying possible team structures before designing architectures that you will never be able to implement.

### Blending Definition and Coding
Steps 7 (Define) and 8 (Code) can occur concurrently. This may happen when you are coding a bounded context, and the insights you get from writing code make you change the high-level design.

## The Process
This process is composed of 8 steps which are introduced below:

### 1. Align
Align our focus with the organisation's business model, the needs of its users, and its short, medium, and long-term goals.

Every decision we take regarding the architecture, the code, or the organisation has business consequences. In order to design, build, and evolve software systems most effectively, our decisions need to create the optimal business impact, which can only be achieved if we are aligned to the business goals.

Badly designed architecture and/or boundaries can have a negative impact or even make it impossible to achieve these goals.

As a starting point, we recommend [The Business Model Canvas](https://www.strategyzer.com/canvas/business-model-canvas).

![The Business Model Canvas](resources/business-model-canvas.png)

#### Tools
- [Impact Mapping](https://www.impactmapping.org/)
- [The Business Model Canvas](https://www.strategyzer.com/canvas/business-model-canvas)
- [The Product Strategy Canvas](https://melissaperri.com/blog/2016/07/14/what-is-good-product-strategy)
- [Wardley Mapping](https://learnwardleymapping.com/)

#### Who to Involve
- Business Stakeholders
- Product Managers
- Project Sponsors
- Senior Management
- Technology Leadership

### 2. Discover
Discover the domain visually and collaboratively.

This is the most crucial aspect of DDD. You cannot skip discovery. If you whole team doesn't build up a good understanding of the domain all software decisions will be misguided.

Spreading domain knowledge through the whole team will create a shared understanding. It enables the developers to build a software system aligned to the domain which can be more flexible to incorporate future business changes. 

Ensuring that domain knowledge is spread across the whole team enables its members to contribute ideas for improving the product.

> #### Discovery is Continuous
>
> Teams who are successful with DDD are practicing discovery techniques on a frequent basis. There is always more to learn about the domain.
>
> When first attempting discovery, a facilitator who is experienced with techniques like EventStorming can help a team to see the true benefits of discovery beyond a superficial level.
>
> We strongly encourage you to check out [Visual Collaboration Tools](https://leanpub.com/visualcollaborationtools).

As a starting point, we recommend [EventStorming](https://www.eventstorming.com/).

![EventStorming](resources/event_storming.jpeg)

#### Tools
- [Domain Storytelling](https://domainstorytelling.org/)
- [Example Mapping](https://cucumber.io/blog/bdd/example-mapping-introduction/)
- [EventStorming](https://www.eventstorming.com/)
- [User Journey Mapping](https://boagworld.com/audio/customer-journey-mapping/)

#### Who to Involve
- Anyone with Domain Knowledge 
- Business Leadership
- Customer Support
- Domain Experts
- Development Team
- Real Users

### 3. Decompose
Decompose the domain into sub-domains - loosely-coupled parts of the domain.

We decompose a large problem domain into sub-domains for a few key reasons:
- reduced cognitive load, so that we can reason about parts of the domain independently,
- give development teams autonomy, so that they can work on separate parts of the solution,
- identifying loose-coupling and high-cohesion in the domain which carries over to our software architecture and team structure.

As a starting point, we recommend [carving up your event storm](resources/event-storm-bounded-context.jpg) into sub-domains.

![Sub-domains on an EventStorm](resources/event_storm_sub_domains.png)*Credit: Alberto Brandolini*

#### Tools
- [Business Capability Modelling](https://www.slideshare.net/trondhr/from-capabilities-to-services-modelling-for-businessit-alignment-v2)
- [Design Heuristics](https://www.dddheuristics.com/)
- [EventStorming with sub-domains](https://www.eventstorming.com/)
- [Independent Service Heuristics](https://github.com/TeamTopologies/Independent-Service-Heuristics)
- [Visualising Sociotechnical Architecture with Context Maps](https://speakerdeck.com/mploed/visualizing-sociotechnical-architectures-with-context-maps)

#### Who to Involve
- Domain Experts
- Product Managers
- Software Architects
- Software Engineers

### 4. Connect
Connect the sub-domains into a loosely-coupled architecture which fulfills end-to-end business use-cases.

It is imperative to not only decompose a large domain into parts but to also carefully design the interactions between those parts to minimise unwanted coupling and complexity. It is necessary to challenge the initial design by applying concrete use-cases to uncover hidden complexity.

As a starting point, we recommend [Domain Message Flow Modelling](https://github.com/ddd-crew/domain-message-flow-modelling).

![Domain Message Flow Modelling](resources/domain-message-flow.jpg)

#### Tools
- [Business Process Model and Notation](https://en.wikipedia.org/wiki/Business_Process_Model_and_Notation)
- [Domain Message Flow Modelling](https://github.com/ddd-crew/domain-message-flow-modelling)
- [Process Modelling EventStorming](https://www.eventstorming.com/)
- [Sequence Diagrams](https://en.wikipedia.org/wiki/Sequence_diagram)

#### Who to Involve
- Domain Experts
- Product Managers
- Software Architects
- Software Engineers

### 5. Strategize
Strategically map out your sub-domains to identify core domains: the parts of the domain which have the greatest potential for business differentiation or strategic significance.

Time and resources are limited, so understanding which parts of the domain to focus on is critical to delivering optimal business impact. 

By analysing what your core domains are, you will have a better idea of how much quality and rigour to each part of your system, and you'll be able to make highly-educated build vs buy vs outsource decisions.

As a starting point, we recommend [Core Domain Charts](https://github.com/ddd-crew/core-domain-charts).

![Core Domain Charts](resources/core-domain-chart.jpg)

#### Tools
- [Core Domain Charts](https://github.com/ddd-crew/core-domain-charts)
- [Purpose Alignment Model](https://www.informit.com/articles/article.aspx?p=1384195&seqNum=2)
- [Wardley Mapping](https://learnwardleymapping.com/)

#### Who to Involve
- Domain Experts
- Business Stakeholders
- Product Managers
- Software Architects
- Software Engineers
- Technology Leadership

### 6. Organise
Organise autonomous teams that are optimised for fast flow and aligned with context boundaries.

We need to organise teams to have autonomy, clear goals and sense of purpose. In order to do that we need to take into account organisational constraints, so that we can organise teams for fast flow. 

We can optimise how people collaborate with each other if we align teams with context boundaries. In order to right-size the teams we need to take into account available talent, cognitive load, communication overhead, and bus factor. 

As a starting point, we recommend visualising sociotechnial architecture with the [Context Maps](https://speakerdeck.com/mploed/visualizing-sociotechnical-architectures-with-context-maps).

![Context Map](resources/context-map.jpg)*Credit: Michael Plöd*

#### Tools
- [Dynamic Reteaming](https://leanpub.com/dynamicreteaming) 
- [Pioneers, Settlers & Town Planners](http://wardleypedia.org/mediawiki/index.php/Pioneers_settlers_town_planners)
- [Team Topologies](https://teamtopologies.com/)
- [Visualising Sociotechnical Architecture with Context Maps](https://speakerdeck.com/mploed/visualizing-sociotechnical-architectures-with-context-maps)

#### Who to Involve
- Human Resources
- Software Architects
- Product Managers
- Senior Leadership

### 7. Define
Define the roles and responsibilities of each [bounded context](https://martinfowler.com/bliki/BoundedContext.html).

Before committing to a design, make explicit decisions about the choices which can have a significant impact on the overall design. Have these conversations early while it is still easy to change your mind and explore alternative models.

Design collaboratively and visually and start to consider the technical limitations so that you can uncover constraints or opportunities. 

As a starting point, we recommend the [Bounded Context Canvas](https://github.com/ddd-crew/bounded-context-canvas).

![Bounded Context Canvas](resources/bounded-context-canvas-v3.jpeg)

#### Tools
- [Bounded Context Canvas](https://github.com/ddd-crew/bounded-context-canvas)
- [C4 System Context Diagram](https://c4model.com/)
- [Quality Storming](https://speakerdeck.com/mploed/quality-storming)

#### Who to Involve
- Product Managers
- Software Architects
- Software Engineers

### 8. Code
Code the domain model. 

Aligning the code to the domain makes it easier to change the code when the domain changes. By collaboratively modelling the problem space with experts, the developers have a chance to learn about the domain and minimise misunderstandings. 

As a starting point, we recommend the [Aggregate Design Canvas](https://github.com/ddd-crew/aggregate-design-canvas).

![Aggregate Design Canvas](resources/aggregate-design-canvas-v1.jpg)

#### Tools
- [Aggregate Design Canvas](https://github.com/ddd-crew/aggregate-design-canvas)
- [C4 Component Diagrams](https://c4model.com)
- [Design-Level EventStorming](https://www.eventstorming.com/)
- [Event Modelling](https://eventmodeling.org/)
- [Hexagonal Architecture](https://en.wikipedia.org/wiki/Hexagonal_architecture_(software))
- [Mob Programming](https://mobprogramming.org/)
- [Model Exploration Whirlpool](https://domainlanguage.com/ddd/whirlpool/)
- [Onion Architecture](https://jeffreypalermo.com/2008/07/the-onion-architecture-part-1/)
- [Unified Modelling Language](https://en.wikipedia.org/wiki/Unified_Modeling_Language)

#### Who to Involve
- Development Team
- Domain Experts
- Software Architects

## Contributors

Thank you to the following individuals who have all contributed to the DDD Starter Modelling Process:

- [Ciaran McNulty](https://github.com/ciaranmcnulty)
- [Gien Verschatse](https://twitter.com/selketjah)
- [Kacper Gunia](https://github.com/cakper)
- [James Morcom](https://twitter.com/morcs)
- [Maxime Sanglan-Charlier](https://twitter.com/__MaxS__)
- [Michael Plöd](https://twitter.com/bitboss?lang=en)
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