---
layout: post
title: Building an effective App Support System
---

As software applications grow, managing bugs effectively becomes paramount. An application support system provides a structured framework for triaging, specifying, and prioritizing incoming bug reports, ensuring prompt and efficient resolution to issues.

This article will go over the necessity for an Application Support System, the core processes of one, common pitfalls, priority levels, and the clear benefits of one.

# The Need for an Application Support

---------------------------------------

Unresolved bugs severely hinder developer output and compromise application stability. Common root causes include technical debt, user errors, and oversights during QA(Quality Assurance) or code reviews.

**The Need**

Without a concrete system of processes to report and prioritize bugs, it will lead to LONG resolution times, resulting in death by 100 papercuts, a term used to describe bugs adding up and ruining the user experience.

**The Business Impact**

Rapidly growing startups and companies operating in domains prone to frequent errors (e.g., web scraping) or critical revenue-impacting bugs (e.g., food delivery and custom framing) particularly benefit from an application support system.

**Typical impact**

-   Slow bug turnaround.

-   Duplicate tickets.

-   Lack of ownership.

-   Productivity loss from the user to the engineer.

Having experience building support systems at startups such as Grubhub, Arcadia, and Framebridge. **Support systems ensure app stability to widen the moat for an exit or IPO**.

## Core Processes
---------------------------

![image of a typical app support request flow diagram from slack](/images/flow-app-support-system.jpg)
*Building Arcadia's Application Support presented at a [monthly All-hands in 2018](https://www.linkedin.com/feed/update/urn:li:activity:6413109425011195904/){:target="_blank"}*

**1. Bug Report**: A user, employee, or monitoring tool submits a bug report, initiating the process. The application support engineer follows up for clarification.

**2. Triage**: Determine the root cause, reproduction steps, and potential workarounds.

**3. Ticket Specification**: Create a detailed ticket with a description, acceptance criteria, original report link, and additional support details.

**4. Prioritization**: Assess business impact, frequency, and related issues to assign a priority level for the current or future sprints.

## Common Pitfalls

----------------------------

- **Duplicate Tickets**: Too many people creating bug tickets can lead to inconsistencies and duplication. Aim for DRY ([Don't Repeat Yourself](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself){:target="_blank"})

- **Lack of Ownership**: The user affected by these bugs should have a clear point of contact, whether an individual or a group.

- **Rotating Software Engineers**: Instead, designate a dedicated role, such as an application support engineer or product manager, to oversee the system.


## Priority Levels

Some companies, like Amazon and Google, use SEV-0 to SEV-4. Naming matters little here, though having common ground is essential to ensure timely resolution.

-  **P0 (Critical)**: Immediate resolution prioritized in the current sprint.

-  **P1 (Major)**: Typically included in the current sprint, based on severity.

-  **P2 (Standard)**: Most tickets, with a chance for the current sprint if necessary.

-  **P3 (Minor)**: Low priority, may be addressed after some time.

## The Benefits

----------------

Implementing an effective application support system streamlines bug management, improves productivity, enhances stability, and creates clarity in a typically cross-functional environment.

By following this framework of processes, even the smallest companies can efficiently manage bugs, promoting a more stable and productive  environment. 

## Conclusion
Overall, it keeps the application effective and stable. Without these core processes set up and pitfalls in view, Arcadia would not be at a unicorn billion-dollar valuation, and Framebridge would not be a market-leading brand in the custom framing industry.

My next post will go over _Building one with $0 using existing features in Slack, Github, and JIRA_.  Thanks for reading!