---
title: "Versioning Standards"
lead: "Set of development rules for Git, Qlik Sense, and Git to Qlik"
date: 2020-10-06T08:50:45+00:00
lastmod: 2020-10-06T08:50:45+00:00
draft: false
images: []
toc: true
weight: 900
---
## GitHub Branches
**The main branch should always be the published application.**  
	 
**Branches should follow naming conventions: name_prefix_feature.**  
For example, hattie_bug_complianceETL. Prefixes are outlined below. Feature should be 1-3 words, camel case, no spaces.
    | prefix | branch type                                            |
|--------|--------------------------------------------------------|
| wip    | Works in progress; stuff I know won't be finished soon |
| feat   | Feature I'm adding or expanding                        |
| bug    | Bug fix or experiment                                  |
| junk   | Throwaway branch created to experiment                 |



Use Pull Requests in your Git provider to merge branches.  
If you are faced with conflicts then use Gitoqlok's load script diff viewer and sheet diff viewer to find the root cause:    
1. Load script diff viewer and sheet diff viewer will highlight differences between versions and helps you to figure out the changes between conflicted versions. 
2. Use Gitoqlok's Import feature to pull changes from another developer to resolve conflicts. 
3. Commit merged version to the branch and create Pull Request again. 
4. If the conflict cannot be resolved, the Qlik team lead (or author of the app) could pull changes from a particular branch into the main branch directly. 
## Working in Qlik