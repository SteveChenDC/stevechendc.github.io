---
layout: post
title: Building an Application Support System
---

An application support system is a group of business processes that handle the triaging, specification, and prioritization of incoming bugs. This article is geared toward startups or small-medium technology companies that have problems closing bugs in a reasonable time and looking for a relatively low-cost fix

|  ![](https://cdn-images-1.medium.com/max/1600/1*WNO95-f9Z2shvxEhnO_4Qg.jpeg)  |
|:--:|
| *This article will cover: who needs one, typical mistakes, and the 4 crucial processes* |

As bug unresolved reports accumulate they start to become a bottleneck in your developer output and overall platform stability. Root causes of these bugs can range from technical debt, user error, and/or oversight of impending bugs that could have been caught in the QA or code review process prior to production release.


>A common reason most bugs aren't fixed in a reasonable time stems from a lack of concrete framework/system to report bugs into an actionable ticket in front of self-organizing engineering team

# Who Needs One and Why?

Typically, **fast-growing startups** that build their own applications and experience rapid uncontrollable growth or work in a domain that results in frequent inconsistent errors(ie. web scraping) or critical revenue costing bugs(food delivery)
For example, in my recent role at Arcadia Power, there were crucial bottlenecks like:
- Bug turnaround time
- Duplicate bug tickets
- Lack of ownership of the tickets
- Engineering productivity loss due to: context switching, annoyances, status updates

This resulted in a decreased satisfaction of non-technical internal teams with engineering
# Some mistakes of existing Application Support Systems
- Multiple ticket creators
- No ownership of the process
- Rotational Software Engineers

These processes typically should be handled by an application support engineer, product manager, or someone who knows the products at a user level to **OWN** the system then make iterative improvements based off feedback and ongoing organizational changes. For the sake of ease, we'll call the person in charge of the system **@app-support**

Another huge mistake startups make is a lack of oversight when asking a software engineer to take in incoming bugs for a rotational day/week/month, don't do this. **Software Engineers are paid to create new code**, typically within their own domains of expertise, not the entire org.

# The 4 Processes of the Application Support System
## Overview
**Bug Report** - A user, employee, or tool reports a bug to be received by someone or something

**Triage** - the process of determining the root causes, steps to reproduce the bug, and workarounds

**Ticket Specification** - Details of the ticket are created and includes: description of the issue, acceptance criteria, and support details

**Prioritization** - Prioritization of the bug within the current sprint and future sprints

|  ![](https://cdn-images-1.medium.com/max/1600/1*mJuBB7YCay0gZ3HcsMLVSw.png)  |
|:--:|
| *How they work. More in the next article* |


## Bug Report
A user, employee, or error monitoring tool sends in a request to kick-off the process, the bug report process is the beginning of it all. The application support engineer or PM follows up with clarifying questions that help in the upcoming processes

## Triage
Immediately after the Bug Report process @app-support determines the following:

- Business impact(customers affected)
- Frequency and Number of reports
- Steps to reproduce
- Known workarounds

## Ticket Specification (& Creation)
The ticket specification process is simply creating the ticket.

Assuming all or most of the Triage process was determined initially* upon the @app-support we can create the ticket in our ticket management platform(JIRA, Github issues, etc) using this template below:
```
**Description**:
**Acceptance Criteria**:
**Original Slack message**:
**Additional Details**:
```


**Description**: Small description of the issue

**Acceptance Criteria**: Criteria for engineers to determine "done"

**Original Slack message**: Link to initial report from Slack(or whatever communication system you use) *Typically you won't have all the details on the initial report, hence why there's an Original Slack Message section to followup

**Additional Details**: Supporting details images, user biases, @app-support's suggestions

## Prioritization
Prioritization phase is where the business impact criteria, from Bug Report process, comes into play. This is the most crucial phase as it decides the fate of the bug and when it should be fixed. Unfortunately, it really depends on an indeterminate number of variables like: number of users affected, how much money the company is losing due to this bug, the implications of other tickets being affected, etc.

This phase entertains the following questions:
- Should we put it in the current sprint?
- How important is this bug to be fixed in relation to every other bug?

> The more comfortable you are with your company's products the higher the likelihood you'll make the right decision

## Prioritization Ratings
In larger and more established organizations these will likely be called something like Sev.

**P0**: Critical. These are extremely rare as they will generally be fixed as it's reported. This is the most crucial ticket and will always be put in the current sprint. These need to be fixed immediately.

**P1**: Major. Typically these will be put in the current sprint, depending on the severity

**P2**: Standard. The majority of tickets will be P2's. These have a decent chance making it into the current sprint, final decision to be made by @app-support or Scrum Master to determine if it's necessary to be fixed this or next week

**P3**: Minor. The rest of the tickets will be P3s. Some will never be touched

# Closing Remarks
Stay tuned for the final article, Part 2 of 2: Implementing an Application Support System - Where I go step by step of what this looks like in a fast growing startup environment(no code required!)


Special thanks to Scott Serok and Chris Vetrano previously from Zoomer