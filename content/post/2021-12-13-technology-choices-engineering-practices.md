---
showonlyimage: true
title:      "Technology choices and Engineering practices"
subtitle:   "Building an Engineering setup in Financial Services - II"
excerpt: "Second batch of the series of 5 posts describing the journey to build Product & Engineering for Financial Services"
description: "Second batch of the series of 5 posts describing the journey to build Product & Engineering for Financial Services"
date:       2021-12-13
author: Amit Kumar
image: "img/home-bg.jpg"
published: true

tags:
    - product engineering
    - engineering at scale
    - financial services
    - engineering excellence
    - infrastructure as a service
    - platform engineering

categories: [ Tech ]
URL: "/2021/12/13/technology-choice-and-engineering-practices/"
---

The second batch of the series of 5 blog posts describing the journey to build an Engineering setup in Financial Services. Read the [preface](/2021/12/02/building-engineering-setup-financial-services/). 

- [Building and scaling Engineering team](/2021/12/07/building-and-scaling-engineering-team/): Principles and practices adopted to build the product and engineering team
- **Technology choices & Engineering practices**: We took an outward-in approach to establish the foundation of technology stack, architecture/design choices & engineering practices
- _Infrastructure_: The core principle was IAC (Infrastructure as Code). We built service oriented structure with Infrastructure as Service
- _Operations - keep the lights ON aka DevOps_: Tranditionally, financial services have a dedicated operations team. Following DevOps principle, we followed -- _You build it, you run it!_
- _Platform Engineering_: A team responsible for engineering tools, cross-cutting-concerns, devops process including SRE. Provide platform-as-service to internal product team.
---

## Development practices

I define good Engineering practices as enablers for shipping good quality software that helps customers and businesses scale (what is the value of writing highest quality code that is not helping your customer). Engineering practices do not need introduction:
- Write testable code with test coverage 
- Run the build and tests in a CI process
- Use test pyramids. Read this {{< link_target_blank href="https://martinfowler.com/articles/practical-test-pyramid.html" title="wonderful article" >}} on Martin Fowler's blog
- Build once, promote further (Deploy automatically or by click of a button)
- Error and exception handling (system, business, integration)
- Make your systems Observable (and auditable)
- Performance and Security are features in the backlog (took a lot of time for us to bring this practice in-place, still WIP)
- Infrastructure and configurations are code (run them in a fully automated pipeline)
- TDD, Code refactoring, architecture/design discussions are mandatory (among these TDD is still WIP)
- Use metrics to measure (extension of DORA)

Like always, we have some guiding principles that was setup, some highlighted ones:

#### Guiding principles:
- **Blue-print the near end state**: always keep the end-state (or the blue-print) in-front. Remember, your end-state **_will evolve_** but it is important to have a path and track the progress. 
- **Align architecture and design principles**: As you scale, to avoid choking design decision-making, it is important to have it distributed but we made sure there is alignment of the ones we care the most:
    - Reusable (don’t reinvent the wheel) and Single source of truth (master)
    - SRP & YAGNI (these are my favorites)
    - Design for Async (least coupling)
    - 
- **Invest in building cross-cutting-concerns** (do an early investment) -- this is the basis of Platform Engineering post (coming soon)
- Reduce entropy - composable architecture
- Organize code and pipelines (automate all components, everything is code)
- Version code/ APIs (use Semver). Document APIs (we used {{< link_target_blank href="https://redoc.ly/" title="Redocly" >}})
- Write single code for all channels (feature parity becomes a big challenge across various channels). We chose Dart (Flutter)
- Follow test pyramid (invest in automation but remember it doesn't solve all testing problems, you still need to do manual testing. Follow measuring ROI)
- **RFCs and ADRs are a must** ({{< link_target_blank href="https://engineering.atspotify.com/2020/04/14/when-should-i-write-an-architecture-decision-record/" title="When should you write an Architecture Decision Record">}})
- **De-couple deployment and release. Feature flag them**
    - Deployments should be as per schedule (we deploy to production at the end of each sprint). Frequent deployments `reduces the blast radius`
    - Enables capabilities for _Canary deployments_ with sophisticated `Feature Flags`
    - Feature release is driven by Product Team based on: feature completeness or other strategies
    ![](/img/deployment-train.jpg "Deployment & Release Train")
- **Always measure your progress with metrics**
As we scale, it is crucial to measure and keep track of the progress & progress. One of the fundamental principle that I learnt from my mentor: `if you have to manage, find ways to measure`. 
Hence, to measure various aspects of our Engineering setup, we defined metrics across various dimensions: