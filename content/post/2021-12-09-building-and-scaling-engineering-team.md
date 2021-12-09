---
showonlyimage: true
title:      "Building & scaling Engineering team"
subtitle:   "Building an Engineering setup in Financial Services - I"
#excerpt: "First batch of the series of 5 posts describing the journey to build Product & Engineering for Financial Services"
description: "First batch of the series of 5 posts describing the journey to build Product & Engineering for Financial Services"
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
URL: "/2021/12/09/building-and-scaling-engineering-team/"
---

The first batch of the series of 5 blog posts describing the journey to build an Engineering setup in Financial Services. Read the [preface](/2021/12/09/building-engineering-setup-financial-services/) to get a clear context of the journey.

- **Building and scaling Engineering team**: Principles and practices adopted to build the product and engineering team
- _Technology choices & Engineering practices_: We took an outward-in approach to establish the foundation of technology stack, architecture/ design choices & engineering practices
- _Infrastructure_: The core principles was IAC (Infrastructure as Code). We built service oriented structure with Infrastructure as Service
- _Operations - keep the lights ON aka DevOps_: Tranditionally, financial services have a dedicated operations team. Following DevOps principle, we followed -- _You build it, you run it!_
- _Platform Engineering_: A team responsible for engineering tools, cross-cutting-concerns, devops process including SRE. Provide platform-as-service to internal product team.
---

## How we started
{{< link_target_blank  href="https://dkatalis.co" title="DKatalis" >}} is an engineering setup. Our tech stack is on the bleeding edge for a Financial services - {{< link_target_blank  href="https://flutter.dev/" title="Dart (Flutter)" >}} for FE, server-side JS (NodeJS) for BE, Kafka (service communication and data streams), APIGW (Tyk), MongoDB, Redis, CloudFlare, ELK, Dynatrace & Solarwinds, Terraform (IAC) & full cloud setup to just name a few.  

Starting to build a team without a brand name is challenging, it starts with your network and expands to layers beyond. Add to it, the bleeding edge of technology (especially Flutter, we couldn't find experienced developers in the region, more on this further), making it even hard to build the team.

> As the {{< link_target_blank  href="https://hbr.org/sponsored/2017/10/guiding-principles-for-closing-the-gap-between-strategy-design-and-delivery" title="HBR post" >}} explains, guilding principles are extremely important to make sure you have a reference point always during execution

Hence, the first step for us was to have guiding principles which will be used to build the team. With help from {{< link_target_blank  href="https://www.linkedin.com/in/maya-kartika-52b2a2131/" title="Maya K" >}} (our Head of People) & {{< link_target_blank  href="https://www.linkedin.com/in/vincentius-ivan-9858581b/" title="Ivan V" >}} (Head of Jakarta Hub), we came up with the following principles:

##### Guiding principles:
- build the team where it is needed
- build the team where talent is available
- responsibilities are more important than title (senior members will have broader set of responsibilities)
- build a balanced team (mix of senior, mid-level & juniors). This is still a struggle for us
- people are assets, invest on them (this is WIP)

With the above guiding principles, it was clear, we need to hire engineers outside Indonesia (although our core business team was in Jakarta). We started the process to establish entities across 3 locations: Singapore, Jakarta & Pune. Not going into details of an entity setup, assembling a diverse & geographically distributed team is tough. The first step was to hire a few good tech recruiters and build network with head hunters. We started with initial 7-8 core members who were tasked to: build the system foundation and also invest time in hiring.

Initially it was slow response but with efforts from our Tech Hub Heads - {{< link_target_blank  href="https://www.linkedin.com/in/vincentius-ivan-9858581b/" title="Ivan V" >}} & {{< link_target_blank  href="https://www.linkedin.com/in/puneet-jain-8133451b" title="Puneet J" >}} and whole recruitment team, we got good results. We grew from 10-12 members in Oct-Nov'19 to 200+ in Dec'20 across the 3 locations -- Singapore, Jakarta & Pune (as of date we have 300+ across the locations).

## The hiring process
One of the fundamental requirement I had put to ourselves (although a challenging one)
> **no matter years of expereince, the person must be hands-on** (this is following our guiding principle #3)

Hence, we configured the hiring process to make sure it reflects the type of team we want to build.

_(with this, we lost a few senior engineers who were not willing to go through the hands-on exercise part, but, I think, it was worth the push during early foundation months)_

![](/img/hiring-funnel.jpg "Hiring Funnel or Stages")

The same process was configured for all the roles: **Product Engineers** (Developers and Automation Engineers), **System Engineers** (Infrastructure), **POs**, **Security Engineers**, **Performance specialists**, **Data Engineers**, **Data Science**, **Data Analysts** etc. This helped to keep consistent hiring process across the organisation. Additionally, it helped propel a culture of roles & responsibilities rather than titles

##### Guiding principles
- Make sure to clearly draft the roles and responsibilities for the profile (aka JD). Confusion there would cost you a lot of recruiter's time.
- Strictly follow the hiring funnel
- Remove subjectivity from hiring
- If in doubt, reject (letting go someone after hiring will be very expensive)
- Keep track of the hiring funnel, fine-tune the process

When you are starting, interviews are the first impression to a candidate (and his network of people) about you and your organisation. Be a **Brand Ambassador** of the company.
Hence, **Candidate Experience** was the first thing to focus. We documented in detail, expectation from each stage of the interview - both recruiters and panelist:
- **how to engage with the candidate (outside and during the interview process)**: intros, pitch about ourselves, explain the hiring process,  pause between questions and invite them to ask, explain about the assignment and the review process, confirm the role he/she has applied
- **scheduling interviews**: recruiter needs to ensure both candidate and panelist are available. They would do an initial intro before the interview starts. If the interview cannot happen, avoid last minute changes
- **how to conduct the interview**: follow guidelines for each stage of the interview
- **during interview**: respect interview time window (review the feedbacks from previous stages and prepare), summarise your understanding (don't assume), be aware of your body language (help them succeed)
- **afetr the interview**: fill feedback form with a defined structure, be available to answer queries from the candidate (even if he/she is not selected), take feedback from the candidate, do a panel debrief, if in conflict

As you grow, the hiring panel starts to broaden and hence, the subjectivity during interviews. Even though, we documented each stage of the interview process, still we started to see subjectivity (or I must say slacks) in hiring - remember we were dealing with hiring at 3 locations and panels. With retro, we found the most challenging was code review, hence, we standardised the code review process. Jeevan D C, Ivan V and I, put clear dimensions for code review feedback: 
- **Code structuring** (Directory structure, First class objects, Modularity, Design patterns)
- **Engineering practices** (Naming conventions, git process/logs, clean coding rules, documentation, tests & coverage)
- **Runtime** (logical approach, error handling, readme)

##### Keeping track of the progress
As you continue to build your team, it is imperative to have a regular review cadence of the progress. The intent is to identify blockers for each stage of the interview and identify opportunities to optimize the process. The first step was to capture data - fall out of profiles from each stage.

> **Waste repellent learning culture - reduce waste, remove unnecessary process**

![](/img/hiring-funnel-breakup.jpg "Percent breakdown for each stage")
The picture above helped us finding opportunities to improve and fine-tune the hiring process, so that we could celebrate successes.

## Organizing teams
As companies scale from 20-100, organizing agile team is a fundamental problem everyone starts to face. I have been part of designing and building engineering Org structure at least twice so far (Bank BTPN during IT Transformation & DKatalis as we scaled). Like always, we established important guiding principles to keep in mind during this process:

- **Reduce silos & increase Communication**: commmunication plays fundamental role between squads. As the number of squads grow, communication or alignment between them starts to break. It can be product spec alignment or prioritisation or design decisions or release dependency. Make sure to define processes to have the communication flowing. More the communication, less the silos across squads.
- **Decouple Org structure & Career growth**: Typically, the boxes of an org structure represents the career path of an individual in an organisation. Additionally, the org structure also becomes the reporting relationships that people might love or hate. We chose to detach Org structure (keep it flat) and Career growth path. Growth path was based on dimensions of responsibility: **Impact, Innovation & Leadership** while the org structure was focussed on pure building blocks of the company. This is an on-going task, we are still working and making it fine-tuned.
- **Customer centricity**: An important dimension of the Org model is {{< link_target_blank href="https://www.forbes.com/sites/strategyand/2015/04/01/10-guiding-principles-of-organization-design" title="value proposition for its customer, employees, investors" >}}. 
- **Team autonomy**: Team autonomy is one of the primary objective for decntralised decision-making. It reduces choke-points and increases team productivity. Like explained by Henrik, team autonomy is one of the fundamental benefits of Spotify model. However, when the number of squads grow, we faced challenges in making sure autonomy is not taken as freedom to choose. So, we introduced what I call {{< link_target_blank href="https://www.linkedin.com/pulse/guardrail-ed-autonomy-amit-kumar/" title="Guardrail-ed Autonomy">}}.
- **Productivity**: The purpose of an Org structure is to enable engineers to be more productive - reduce blockers, increase collaboration. In the new batch of the series, I explain in detail about the Development practices and processes that helped us with productivity.

#### Tribes-Squads-Chapters
{{< link_target_blank href="https://www.atlassian.com/agile/agile-at-scale/spotify" title="`Spotify Model`" >}} answers most of the guiding principles listed above, hence, it was our defacto choice to organise the team. Having said that, Spotify model doesn't answer many questions, so, we didn't consider 

> Spotify model as a framework 

(as suggested by Henrik Kniberg in his article {{< link_target_blank href="https://blog.crisp.se/2015/06/07/henrikkniberg/no-i-didnt-invent-the-spotify-model" title="No, I didn’t invent the Spotify model" >}}) but as guidelines for autonomy, communication, accountability, and quality. 

We organised ourselves in sqads & chapters.  

![](/img/squad-structure.jpg "Squad Structure")
A typical squad would be lead by a combination of PO and Tech Lead (who are also responsible for the scrum ceremonies). Additionally, a squad will also have FSE - Full Stack Engineers (each specialising in FE or BE) and Quality Engineers. We tried to maintain a healthy ratio of 3:1 (for every 3 developers, 1 QE). I have my opnion about FSE, it's a myth that an Engineer can be an all-rounder - who can specialise in FE, BE and Systems - _opinion for another article_. Our approach has been to pair FE and BE devs together to optimise productivity and during this process they get to learn from each other. Additionally, we also did some bootcamps for Flutter (for BE Engg) amd NodeJS (for FE Engg).

![](/img/squads-chapters.jpg "Squads and Chapters")
If you haven't read about Squads and Chapters {{< link_target_blank href="https://www.atlassian.com/agile/agile-at-scale/spotify" title="Discover Spotify Model">}}

We built some core squads responsible for specialised work:
- **Platform Engineering** (_more on this in the upcoming post_): they are responsible for: cross-cutting concerns, tools/platforms/components are re-used across all tribes & squads etc.. in short they are glue between Product Delivery and Infrastructure squads.
- **Samurai**: A specialised squad responsible for managing Automation frameworks, Performance/ Load test frameworks, DevSecOps 
- **Sniper**: A squad responsible for providing IaaS to all other squads. They do: IAC, Infra operations, Monitoring, Alerts.
![](/img/org-structure.jpg "Oragnisation Structure")

> what was not working well

The model worked beautifully for 8-9 squads but as we started to scale, we started to see issues with: communication across squads, prioritisation, alignment of practices, architecture decisions, cross-cutting common components, observability - to name a few. Like I said, to solve we had to introduce processes in-place - will explain at in the practices article next.

#### The upskilling program
Or rather capability building - we designed a number of bootcamps and upskilling programs to make sure everyone can take out time to learn. Some are listed below:
- best practices for writing good quality software
- good practices for wirting & managing backlogs (including cross-squad alignment)
- how to effectively use OKRs to manage priorities and cross tribe/ squad dependencies
- devops bootcamps

## Pitfalls and learnings
It was a great learning experience building a setup from ground zero and scale to 300+ in less than 2 years. For sure, we made many mistakes but learnt immensely during this journey. Some of the important ones to highlight here:

- **Build Platform Engineering squad** :+1:: Do an early investment in shaping Platform Engineering Squad and make sure they have right capacity. We did so and hence, we repeaed benefits of having:
    - reference blue-print of the architecture
    - cross-cutting concerns (reusuable modules & boiletr-plate code) were developed before product squads started to write features. This heplped in reducing the sphagetti of code duplication and inconsistency across various squads
    - focussed attention on non-functional features - performance, scalability, reliability, security
- **Hiring mistakes are very expensive** _- build a balanced team_ :-1:: this is one of the problems that we are still solving. We hired quite a few junior staff, although, we designed bootcamps and crash-courses to bring them up-to-speed, but it still takes time for them to indepedently productive
- **Avoid cross-squad feature split** :ok_hand:: As far as possible, do a full vertical slice of feature to a squad (FE, BE, Systems, Operations). Distributing it across multiple squads leads to un-necessary project management overheads
- Chapters should be tightly integrated with the Product Backlog, otherwise, chapters would just be on paper :-1:
- **Measuring productivity of squads is a trap**, rather focus on outcomes they are producing:
    - You should never compare velocity of multiple squads (this is a well known fact) but we end up doing that. Very soon it becomes a number game and the squads will start to blow-up story points to match up velocity (:-1:)
    - Define other metrics to measure outcome from squads:
        - quality metrics
        - time to ship a feature
        - incidents or bugs found on production
        - bug to story ratio
        - life of critical bug on production
    are goode examples of outcomes produced by squads. In the next article I would walk through classification of such metrics.
- **Have a regular cadence of sessions with the whole Organisation** :ok_hand:: share the larger picture, celebrate successes & learnings
- **Designing career path/ growth** is tough :-1:. Do early investment

I hope this article was an interesting read and provided good insights on my journey building an Engineering team.

---
People talk a lot about Engineering culture, however my strong belief is: 
`practices followed in the organisation gets into DNA and hence becomes the culture`
I would like to hear your thoughts on Engineering Culture and ending this article with the statement:
> **Engineering culture (or rather any culture) is an outcome of practices followed by them**

_(more on this in a separate article)_