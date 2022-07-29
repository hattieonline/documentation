---
title: "Dashboard Use Cases"
lead: "TLDR: Identify the user. Identify the user's goals. Write down actions for that goal."
date: 2020-10-06T08:50:45+00:00
lastmod: 2020-10-06T08:50:45+00:00
draft: false
images: []
weight: 20
---


## Overview
A use case describes a specific business goal to be satisfied by, in this case, Insights dashboards. It outlines, from a user’s point of view, a related sequence of steps (a
scenario), for the purpose of completing a single business task. Each use case is represented as a sequence of simple steps, beginning with a user's goal and ending when that goal is fulfilled.  

### Elements of the Use Case
**Name:** Like business processes, use cases are named verb-noun style. The name indicates what action the user is taking to be described in the use case. For a basic (and not actually useful) example, "Discover Birthdays" rather than "The Resident Birthday Use Case"  

**A brief description:** 1-3 sentence blip that summarizes the use case and gets clear about the scope. Define specifically the goals of the primary user of the system. Outline the process, focusing on two sentences: *this use case starts when...* and *this use case ends when...* Think K.I.S.S (Keep It Stupid Simple).

**Actors:** The users, or roles, that may use the dashboard. It’s not specifically about job title; multiple people can fill that role with the system. It’s what the system can identify about you. Are you in a community-level sales role? Are you in the c-suite?  

**Preconditions and/or Triggers:** Preconditions outline what the system knows to be true, before the use case starts. Triggers prompt the user to begin the process.

**Expected Outcome:** The final successful outcome that completes the process.  

**Basic Flow:** The process and steps the user takes to accomplish a particular task, including the necessary functional requirements and their anticipated behaviors. Think of basic flow like a ping pong game. The user does one thing, the app does another thing. The user does one thing, the app does another thing. It doesn’t have to be just one back-and-forth like that, but thinking about it as ping pong helps make sure that you’re getting that user-system interaction.  

Be careful to avoid the technical details of what the system is doing. It’s not a technical specification. It’s not a system specification. You want the requirements. What’s the observable piece of the dashboard that the user can see and experience it doing? Not *how* the dashboard is doing all of it.  

**Alternate and Exception Flows:** Alternate flows explain less common actions. Exception flows detail what happens when the user cannot achieve the goal.



### Characteristics 
1. Organizes functional requirements.
2. Models the goals of system/actor interactions.
3. Records paths -- called scenarios -- from trigger events to goals.
4. Describes one main flow of events and various alternate flows.
5. Multi-level, so that one use case can use the functionality of another one.  

## Suggested Methodology
Approach first from dashboard-level perspective. Each sheet has its own workflows and use cases, but they work together, cohesively, in one dashboard that serves a greater purpose. Given that sheets contain a set of related visualization objects, use-cases will typically align with sheets naturally, with room for overlap and commonalities (see characteristic 5).
### Define the purpose and scope
1. Identify stakeholders. These are the people in the organization who care about the outcome of the process. They may not be users in the process described by the use case, but the system acts to satisfy their interests.
2. Define what is in and out of scope. Specifically identify the system that is being evaluated, and leave out elements that are not part of this system. It may be helpful to create an In/Out list. First, list any topic at all that may relate to the system. Then, categorize each item in the list as "in" or "out". If it doesn't happen in the system at hand, it needn't be included. System, here, could refer either to a dashboard or a sheet, depending on the scope of your use case. 
3. Write a goal statement for each actor.
### Write the use case steps
1. Define all actors/end users.
2. Define how each actor will use the technology or process-- what goals could they want to accomplish? Each thing the user does becomes a separate use case. For example, in Care - Tasks, one use case may be analyzing resource allocation, another may be identifying residents in need of reassessment. 
3. Name each use case and write a brief description.
4. Describe the normal course of action taken within the dashboard to reach that goal. Outline everything the user does and how the process responds to those actions.
5. Consider every alternate course of events, and extend the use case. Alternate flows and exception flows are written to describe the actions when there are obstacles to the goal.
6. Repeat steps 1-6 for all other dashboard users.

## Tips for Ideation
Start by thinking about why businesses implement BI and what their goals are, then consider how your dashboard or sheet helps the business to reach that goal.

**1. Early warning on business problems by tracking and analysis of KPIs**  
BI reporting is about adding dimension to those KPIs so they may be ranked or provide context. What KPI will the user want to see? What will the user want to investigate? 

**2. More informed decision-making by business executives and users**  
What kinds of decisions could the user want to make based on the data? What events have occurred that they will want to evaluate? Could they use this information to predict likely outcomes in the future?  

**3. Operational improvements in departments and business units**  
What kinds of inefficiencies in the business process could be identified? How could they track down things that are running amiss? Could they uncover any operational dynamics that need attention?  

**4. More effective sales campaigns to lower costs and boost sales**  
What insights can be gleaned about the needs, wants, and purchasing patterns of existing and potential customers? What's working? What isn't?  

