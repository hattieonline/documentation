---
title: "Git-to-Qlik"
lead: "WORK IN PROGRESS: Insights dashboard versioning using the extension Git to Qlik."
date: 2020-10-06T08:50:45+00:00
lastmod: 2020-10-06T08:50:45+00:00
draft: false
images: []
toc: true
weight: 100
---

Gitoqlik is a Chrome browser extension that connects Qlik Sense to GitHub, and lets you save your applications in repositories. **[Install it here](https://chrome.google.com/webstore/detail/gitoqlik/kkgicbgpgfcbhcbmifmfagggnpkebdaj)**. 
It versions both the visual objects and data load script directly from the web-browser, as well as provides the ability for developers to collaborate together and share their best practices via public or private GitHub.


# A working example
Source: [How to use git with Qlik Sense](https://apolorotov.medium.com/how-to-use-git-with-qlik-sense-part-1-3af14e03cac3)   





Say hello to **John**, **Adam**, and **Eve**.‌ **John** is a Qlik Sense Data Architect.  
**Adam** and **Eve** are amazing data visualization experts who are certified Qlik Sense Business Analysts.
1.  **John** is taking care of the data models and the ETL-process development.
2.  **Adam** and **Eve** are handling the visualizations and sheets for the Qlik Sense application.
3.  **The team has decided to use GitHub** to track the client’s requirements and to version control the application source code.‌  
|
|:--:|
| ![](https://miro.medium.com/max/250/1*406fwZyeMCyNYH76WF16VQ.png)





As the ETL process has been taken care of, John creates an application and builds out the data model for Adam and Eve to use. We’ll call this application **the master application.** 
 John **creates a GitHub repository using Gitoqlik** and gives access to Adam and Eve.
A repository is a version-controlled storage space for your application, and the JSON files that represent your application. This is done by clicking the “Create a repository” button inside of Gitoqlik.

| ![](https://miro.medium.com/max/500/1*vXUsvRTPzUMalg5O5kFjpQ.png) |
|:--:|
|“Create a repository” button inside of Gitoqlik.

Gitoqlik **will automatically create a master branch**, which **is the main branch for the repository**. A branch is a specific starting state of the contents of a repository. The state can be further altered with new changes or reverted to an older version of itself.‌

As John is developing the application and the data models, he commits (saves and sends) his changes into the repository. This commit history is saved as a changeset by Git and can be restored to any previous state. John can revert changes if things in his application are not functioning properly.

> A branch is a specific starting state of the contents of a repository. The state can be further altered with new changes or reverted to an older version of itself.



| ![](https://miro.medium.com/max/500/0*AdSbarCYB0v4M3UP) |
|:--:|

As soon as John is done with his work he’s ready to pass the ball into Adam and Eve’s court. He does this by publishing his application into the “STAGE-3” stream in Qlik Sense. Adam and Eve copy the application into their workspaces.‌

They now **have two copies of the master application** and **they will each develop their sheets**. Before beginning, Adam and Eve plan to divide the work between each other.
Adam will be developing Pivot table sheets and ABC-analysis sheets.
‌Eve going to create the “KPI” and the Custom report sheets.

| ![](https://miro.medium.com/max/400/1*HUYAf6FXEgkAcOgIlj05Kw.png) |
|:--:|




Adam needs to create an isolated branch inside the repository. This way all his changes are not recorded in the master application “master” branch but in a separate one. He uses Gitoqlik and connects to his GitHub account. Gitoqlik automatically detects copies of the application and finds the relevant master application repositories.

| ![](https://miro.medium.com/max/460/1*kZzzWM-AYpYw8_svpJkh2A.png) |
|:--:|






| ![](https://miro.medium.com/max/700/0*L42PkpXLMyd8HrKz) |
|:--:|
|This is what the commit-graph would look like once Adam begins to work.



| ![](https://miro.medium.com/max/700/1*0EPvJnfHGCzwCzVNO4FQRQ.jpeg) |
|:--:|
|Eve does the same





| ![](https://miro.medium.com/max/700/1*Dk2f1jqBy-Wf2SJ3d81qxw.jpeg) |
|:--:|
|They continue to work separately on their sheets while committing to their own branches for the application.


Once they’re both done, the team is ready to merge the branches in the master application repository. Both Adam and Eve create pull requests to merge their branches into the master branch. This is usually done through the console terminal or using standalone and IDE-bundled GUI tools. We’ll be using GitHub for this, though.


| ![](https://miro.medium.com/max/700/1*ZrGcxH9w8-o_CsdbqZGTVQ.png) |
|:--:|
|After accessing the repository page on GitHub we need to click **the “Compare & pull request”** button and follow the on-screen instructions.




Once Adam and Eve have created their pull requests John, being the repository owner and the one responsible for the master branch and merges into it, accepts Adam’s and Eve’s work. The commits become part of the master branch.

| ![](https://miro.medium.com/max/1400/1*ORNjamgj9z72t2zxRFQFRA.gif) |
|:--:|
|The resulting state of the master branch contains all the changes from Adam’s branch and all the changes from Eve’s branch.





| ![](https://miro.medium.com/max/700/1*ugE5GsNkR059i1cncgbayQ.jpeg) |
|:--:|
|John can now checkout their work to update the state of his local repository.


| ![](https://miro.medium.com/max/80/0*TO-Ff-qR5nxY90ho) |
|:--:|
|If you see this icon you are in the out-of-date version of the application. Don’t forget to update your state.


Gitoqlik will show available updates that can be applied to the master application state. To do this John clicks the “Update” button and can get the latest state of the repository and the application, which includes the work done by Adam and Eve.

![](https://miro.medium.com/max/1400/1*aSYhVWOxPCR6ai0auMI8dQ.gif)

So, Gitoqlik allows developers to work in isolated environments without the usual back and forth that collaboration without Git requires. The work can then be easily merged without trying to figure out which changes need to be copied where. Version control makes Qlik Sense development manageable and smart with the help of Git.


