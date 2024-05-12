---
layout: post
title: Building an Application Support System
---

As software applications grow in complexity and usage, having a robust system for managing bugs and issues becomes crucial. This article outlines a framework for establishing an application support system tailored for startups and small-to-medium technology companies seeking to streamline their bug resolution processes.

Why You Need an Application Support System
------------------------------------------

Unresolved bugs can quickly become a bottleneck, hindering developer productivity and compromising platform stability. Common root causes include technical debt, user errors, and oversights during the QA or code review phases. Often, the lack of a structured system to report and prioritize bugs leads to prolonged resolution times.

Rapidly growing startups and companies operating in domains prone to frequent errors (e.g., web scraping) or critical revenue-impacting bugs (e.g., food delivery) can particularly benefit from an application support system. Typical challenges include:

-   Slow bug turnaround times
-   Duplicate bug tickets
-   Lack of ticket ownership
-   Engineering productivity loss due to context switching, interruptions, and status updates
-   Decreased satisfaction of non-technical teams with engineering

Common Pitfalls to Avoid
------------------------

Successful implementation of an application support system requires addressing common mistakes, such as:

1.  **Multiple Ticket Creators**: Having too many people creating bug tickets can lead to inconsistencies and duplication.
2.  **Lack of Ownership**: Assigning application support responsibilities on a rotational basis to software engineers can be ineffective, as their primary role is writing new code within their domains of expertise.
3.  **Rotating Software Engineers**: Rather than rotating software engineers through application support duties, designate a dedicated role, such as an application support engineer or product manager, to oversee the system.

The Four Crucial Processes
--------------------------

An effective application support system comprises four core processes:

1.  **Bug Report**: A user, employee, or monitoring tool reports a bug, initiating the process.
2.  **Triage**: The application support engineer determines the root cause, steps to reproduce the bug, and potential workarounds.
3.  **Ticket Specification**: A detailed ticket is created, including a description, acceptance criteria, and support details.
4.  **Prioritization**: The bug is prioritized based on its business impact, frequency, and other factors, determining its place in the current or future sprints.

### Bug Report

The bug report process kickstarts the application support system. A user, employee, or error monitoring tool submits a report, which the application support engineer or product manager follows up on with clarifying questions to aid the subsequent processes.

### Triage

During triage, the application support engineer aims to understand:

-   Business impact (customers affected)
-   Frequency and number of reports
-   Steps to reproduce
-   Known workarounds

### Ticket Specification

With the triage information, a detailed ticket can be created in the ticketing management system (e.g., JIRA, GitHub Issues). The ticket should include:

-   **Description**: A concise summary of the issue.
-   **Acceptance Criteria**: The criteria engineers use to determine when the ticket is resolved.
-   **Original Report**: A link to the initial bug report for reference.
-   **Additional Details**: Supporting information, such as images, user biases, or suggestions from the application support engineer.

### Prioritization

Prioritization is the most crucial phase, as it determines when the bug should be fixed. Factors like the number of affected users, potential revenue loss, and the impact on other tickets influence the priority level assigned. The application support engineer or product manager should be well-versed in the company's products to make informed decisions.

Typical priority levels include:

-   **P0 (Critical)**: Extremely rare, these bugs require immediate resolution and are prioritized in the current sprint.
-   **P1 (Major)**: Usually included in the current sprint, depending on severity.
-   **P2 (Standard)**: The majority of tickets fall into this category, with a chance of being addressed in the current sprint based on necessity.
-   **P3 (Minor)**: Lower-priority tickets that may not be addressed immediately, if at all.

Conclusion
----------

Implementing an effective application support system is crucial for maintaining high-quality software and ensuring efficient bug resolution. By following the outlined framework and avoiding common pitfalls, startups and technology companies can establish a streamlined process for managing bugs, promoting developer productivity and customer satisfaction.