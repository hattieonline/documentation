---
title: "Backlog"
description: "Backlog and Roadmap"
lead: "Backlog and Roadmap"
date: 2020-08-27T19:25:12+02:00
lastmod: 2020-08-27T19:25:12+02:00
draft: false
images: []
toc: true
---
Documentation project backlog. Known issues, upcoming enhancements.
## To Do
### Fix metadata error with Performance Analytics and Trends

**Current state:** a sheet in Performance Analytics causes the PowerShell ETL scripts to fail. Thus, Sales Performance Analytics and Sales Trends (the only app loaded into PowerShell after Performance Analytics) have incomplete documentation pages.

**Desired state:** Identify cause of issue and a workaround? I believe this is due to a hyphenated title.

**Priority**: High

**Effort Type:** PowerShell

**Epic:** JSON ETL

**Item Type**: Known issue

### Searchable App Contents

**Current state:** app and app descriptions are the only items searchable via site search bar.

**Desired state:** measures, dimensions, load scripts, chart titles should also be searchable.

**Action plan:** Transform app JSON into format needed for FlexSearch.js and append logic to Index.js to access this JSON
[https://github.com/nextapps-de/flexsearch#complex-documents](https://github.com/nextapps-de/flexsearch#complex-documents)

**Effort Type:** Web development

**Priority:** High

**Epic:** Documentation

**Item Type:** Enhancement

### TOC for templated data

**Current state:** table of contents is not populating for documentation page headers (sheet objects, measures and dimensions, load scripts). One must scroll to get to desired section.

**Desired state:** TOC for one-click section navigation

**Action notes:** Either a) working with front matter and sections (Hugo) or b) adjusting Index with logic to conditionally show. If B, this is a good opportunity to implement header logic — ex: not showing "Sheet Objects" on ETL apps.

**Priority:** Medium

**Effort Type:** Web development

**Epic:** Documentation

**Item Type:** Enhancement

### Update JSON-ETL

**Current state:** JSON ETL loads repositories from a folder, runs through ETL scripts, deposits that data into documentation data store. This file paths are outdated and some steps are redundant.

**Desired state:** Update file path for new workflow — adjust root directory, remove logic that creates folders, ensure file names use sheet ID and not name (or at least use a definitively unique identifier)

**Priority:** Medium

**Effort Type:** PowerShell

**Epic:** JSON ETL

**Item Type:** Workflow Step

### Front end UI customizations

Customizations to documentation UI.

**Current state:** uses default theme colors, font, navigation, footer.

**Desired state:** customize SCSS variables, update font, "Keep it stupid simple" principles to any non-data pixels (remove clutter)

**Priority:** Medium

**Effort Type:** Web development

**Epic:** Documentation

**Item Type:** Enhancement  

-  [x]  update index.html
- [ ]  correct colors in SCSS vars
- [ ]  replace font
- [x]  update footer
- [x]  remove twitter icon

### Append heading logic to AppData partials

**Current state:** Even if an app has no sheets, there are still page headers for measures/dimensions and sheet objects.

**Desired state:** only show headers if data exists

**Priority**: Low

**Effort Type:** Web development

**Epic:** Documentation

**Item Type:** Known issue

### Implement WYSWIG with GitHub

**Current state:** static content updated in VSCode

**Desired state:** add "Edit" button to documentation pages that directs user to the corresponding file in GitHub repository

**Priority:** Low

**Effort Type**: GitHub

**Epic**: Documentation

**Item Type:** Enhancement

### Readable format for charts titled with expressions

**Current state**: Charts that use expressions in titles are shown in documentation within a nested array and are not very readable

**Desired state**: Implement logic in PowerShell ETL that displays expression titles in a comprehensible format.

**Priority:** Low

**Effort Type**: PowerShell

**Epic**: JSON ETL

**Item Type**: Known issue

### Site navigation and menu bug

**Current state**: When navigating published site, deleted menu items are still present in navigation bar and old versions of the site are displayed.

**Desired state**: published site has cohesive navigation & definitively identify the cause of this and a solution

**Priority:** High

**Effort Type**: Web development

**Epic:** Documentation

**Item Type**: Known issue

### Temp: search of load scripts

An important part about this documentation is that it should inform analysts which apps load which fields from which tables.

**Current state:** load scripts are partitioned by app and are not currently searchable via search bar.

**Desired state:** Until searchable scripts are implemented, add a page which contains all app load scripts so that we may CTRL F to search.

**Priority**: High

**Effort Type**: Web development

**Epic**: Documentation

**Item Type**: Enhancement

### Temp: search of measures

Until searchable measures and dimensions are implemented, create a new page that contains all measures, by app, so that they may be searched in the interim

**Priority:** High

**Effort Type:** Web development

**Epic:** Documentation

**Item Type:** Enhancement

## Done

### Deploy Iteration #1 of Analyst Documentation

**Priority:** High

**Effort Type:** Web development

**Epic:** Documentation

### Fix error with ADL populating Transformation page

**Priority:** Medium

**Effort Type:** PowerShell

**Epic:** Documentation

### Fix duplication of sheet objects in app pages

Priority: High

Effort Type: PowerShell

Epic: JSON ETL

### Future plans
Complete this page?