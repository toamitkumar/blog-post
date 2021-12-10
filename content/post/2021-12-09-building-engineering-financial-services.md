---
showonlyimage: true
title:      "Building an Engineering setup in Financial Services"
subtitle:   "A series of 5 posts describing the journey to build Product & Engineering for Financial Services"
excerpt: ""
description: ""
date:       2021-12-09
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
URL: "/2021/12/09/building-engineering-setup-financial-services/"
---

I have been part of building Product & Engineering teams and Digital Transformation setup for almost more than a decade. 

My first experience was during the build of MDL (McKinsey Digital Labs) by our leaders: {{< link_target_blank  href="https://www.linkedin.com/in/sattybhens" title="Satty Bhens" >}} and {{< link_target_blank href="https://www.linkedin.com/in/bijubhaskar/" title="Biju Bhaskar" >}} - a startup like setup (for both engineering setup and business building) inside a large organisation.
They both are strong believers of garage-like setup and gave full support to establish guard-rails in protecting the culture of working like a startup.
Together, we built a solid team of 150+ engineers globally following {{< link_target_blank  href="https://en.wikipedia.org/wiki/Spoke%E2%80%93hub_distribution_paradigm" title="hubs-spokes" >}} model knitted together with an **Engineering Mindset** & connected via various communication tools.

### Last life
In my last journey, I have been part of Digital Transformation for {{< link_target_blank  href="https://www.btpn.com/en" title="Bank BTPN" >}}. 
The whole transformation (Technology, Agile & People) journey in the bank is a long story **_for another post_**. But, it was great to **replicate building a garage-like-setup** (although it was not a global setup) - with ring-fenced teams dedicated for each digital product offerings in the bank. The setup was driven by guiding principles: customer focussed squads, solid development practices for building product, devops mindset, infrastructure as a service (with IAC), observability-enabled systems, to name a few.

From an Engineering lens, during this journey, we faced many challenges (nothing surprising), describing a few:

- attracting and retaining [**digital talent**](https://www.gartner.com/en/human-resources/insights/talent-in-digital) to work in a bank is challenging. A majority of them enjoy working with Fintechs or start-ups
- implementing engineering innovation within the boundaries of a bank (_a highly regulated entity_) is challenging. Simple things like automated deployment (_without manual intervention_) requires compliance/regulatory approvals or using monitoring tools like NewRelic required a lot of back-n-forth (not to mention cloud or cloud-based SaaS providers)
- infrastructure (bare metal) becomes hinderance for rapid scale. You need native cloud setup to enable Infrastructure scale with flexible cost. _We used Openshift for a cloud native setup - story for another day_. {{< link_target_blank href="https://aws.amazon.com/outposts/" title="Outpost (AWS)" >}}, {{< link_target_blank href="https://aws.amazon.com/outposts/" title="Anthos (GCP)" >}}, {{< link_target_blank href="https://aws.amazon.com/outposts/" title="Stack (Azure)" >}} help solve these problems to provide a more cloud friendly environment.

There were other challenges as well - customer acquisition, GTM strategy, regional growth, to name a few... 

### What I am doing now

Hence, in the new journey of building a technology-based Financial Services - {{< link_target_blank href="https://dkatalis.co" title="DKatalis" >}} (Digital Katalis, Katalis is a Sanskrit word which means Catalyst), we leaped to set an Engineering organisation that would provide services to a Bank (in Jakarta, Indonesia). 

I am writing down a series of posts explaining various aspects of the journey in building Product & Engineering setup outside (or at arms-length) from the highly regulated entity.

The posts covers:

- [Building and scaling Engineering team](/2021/12/09/building-and-scaling-engineering-team/): Principles and practices adopted to build the product and engineering team
- _Technology choices & Engineering practices_: We took an outward-in approach to establish the foundation of technology stack, architecture/  design choices & engineering practices
- _Infrastructure_: The core principle was IAC (Infrastructure as Code). We built service-oriented structure with Infrastructure as Service
- _Operations - keep the lights ON aka DevOps_: Traditionally, financial services have a dedicated operations team. Following DevOps principle, we followed -- _You build it, you run it!_
- _Platform Engineering_: A team responsible for engineering tools, cross-cutting-concerns, devops process including SRE. Provide platform-as-service to the internal product team.
---

It will be great to hear your thoughts, ideas - if you've been on a similar journey.