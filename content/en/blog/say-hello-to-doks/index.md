---
title: "Project Roadmap"
description: "Review of current and planned directions for analyst documentation."
excerpt: "Review of current and planned directions for analyst documentation."
date: 2020-11-04T09:19:42+01:00
lastmod: 2020-11-04T09:19:42+01:00
draft: false
weight: 50
images: []
categories: ["Updates"]
tags: ["documentation",  "roadmap"]
contributors: ["Hattie Sager"]
pinned: false
homepage: false
---
 
**Processes, Policies, Procedures | Confluence**  
Processes, policies – anything that does not involve the current inner-workings of a specific app – will be maintained in Confluence.

**Dashboard Documentation | GitHub Pages**  
App metadata – searchable information about apps, sheets, charts, dimensions, measures, fields, and load scripts, integrated with GitHub for automated updates to documentation as apps are updated.

## BI Documentation Using Confluence

**Operations**

1.  BI Processes  
General guidelines and policies relating to Insights BI – versioning, fielding requests, project scoping, UAT, publishing apps, etc.
    
    
    
2.   Technical Procedures  
Automations with Microsoft Flow, script library / tutorials for PowerShell, Qlik CLI, etc. API reference for Jira.
    
   
    

**Guidelines**

1.  UX/UI  
Design system and semantic notation
    
    
    
2.   Data Modelling  
Scripting standards and best practices
    
   
    

**Resources**

1.  Collaboration Sandbox  
Team notes, helpful online resources, maybe sprint planning and retro?
    
    
    
2.  Dashboard Documentation  
Documentation on site maintenance and operation.
    
    
    

## Web-Hosted Dashboard Documentation

### **Iteration #1: Fundamentals and currently accessible pathways** Provide information about out-of-box dashboard objects and scripts.

**As an Insights analyst, I would like to:**

1.  View all fields *in use* in an app  
*So that I can identify applications in need of updates due to changes in source data, or optimize app performance by eliminating fields not in use.*
    
    
    
2.  Quickly locate information about measures and dimensions in a specific app  
*So that I can provide support, identify discrepancies for standardization, without duplicating an app*
    - I want to navigate to a specific app to view a specific measure  
    - I want to search for a measure and locate where it is used
    
    
    <br>
3.  Be informed about the location and contents of reports offered by Insights  
*So that I can provide support, field redundant requests, and understand the purpose and contents of each chart object provided by Insights.*
    
    - I want to know if a similar report to the one requested already exists, if the fields I need in order to fulfill the request are already loaded into the app, if the report has matching access, which stakeholder I should consult.  
    <br>

    
4.   Access standardized assets used throughout multiple Insights products, such as load scripts and measures  
        - I want to find the dimDate load script   
        - I want to know if a certain field is in the factInquiryByReferral table  



    
   
    

### Iteration #2: Incorporation of human-generated or extraneous detail

**Identify and collect the pertinent app information that lives in our heads**

1. Identify subject matter experts
    - I want to know who the business stakeholder is for this app.
    - I want to know if there is an “owner” of this app that I should consult with about changes.  
    <br>
2.  Shed light on obscure logic and dispel any assumptions
    
    - I want to feel equipped to make adjustments to an app that I am not very familiar with.
    - I want to know if this logic is in place for a reason, the reason, if it may be changed, and who requested it be put in place.
    - I want to know if and what I should be wary of when developing in the app.

**Author, revise, and publish information to analyst documentation**  
*Note: this should happen in tandem with standardization process.*

1.   Update each dashboard’s documentation landing page  
Include higher level information such as subject matter experts or general app notes to enable other analysts for rapid and reliable development. Make note any object logic that cannot be detailed in the user-facing descriptions.
    
   
    
2. Update each Insights dashboard  
 Add comments to complex load script logic, update object descriptions with explanations of logic that the end-user can or should see.
    
    
    

**Incorporate metadata from GitHub**

1. I want to view a changelog of app contents – what changed, who changed it, what was it previously, and why was it changed?
2. I want to know how many branches of this app exist, and what are the customer configuration variances?

### Iteration #∞ Documentation Roadmap: Integrations & Future Direction

**Implement GitHub versioning across all customer environments**

1. I want to view customer-specific app documentation
2. I want to compare app contents across multiple customers

**Utilize data from Qlik**

1. Connect to REST APIs    
    I want to see a sample of data values, because I’m not sure what this dimension is.
    I want to know when a task reloads, what is the trigger, and when it last reloaded  
    I want a general audit of user access – which groups have access  

2.  I want to view utilization KPIs alongside app information, and I want drill down to chart-level metrics.
3. Implement and access data from monitoring apps
    

**Implement complex site navigation and logic**

1.   Create links between chart objects, app fields, and script contents  
 So that I can navigate through the dependencies of expressions and load scripts to identify source logic.  
 *ie. this measure uses that field, that field is loaded from this fact table, that fact table is in this section of the transformation, which transforms that field using this logic, and bonus: that logic was put in place by this stakeholder*
    
  
    
2.  Implement WYSIWYG functionality  
I want to easily update static information – stakeholders, notes on app operations, and dependencies – without needing any technical know-how.
    
    