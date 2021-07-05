---
tags: Architecture Dashboard.
summary: Learn how to check the technical debt of your team's apps.
en_title: Getting started as a team lead
---

# Getting started as a team lead

As a team lead, the Architecture Dashboard provides you with an overview of the technical debt of organization's technical debt as well as detailed overview of the technical debt of your teams’s apps. From the canvas, you can drill down into the team's problematic modules, and take the necessary steps to reduce the technical debt score for these areas. 

This guide assumes the following:

* Your infrastructure is already set up in Architecture Dashboard.

* Your IT user is already associated with Architecture Dashboard.

After logging in to [Architecture Dashboard](https://architecture.outsystems.com) with your OutSystems account, follow these steps:

### Check the technical debt of your team apps

The canvas gives you an overview of all the apps on your infrastructure.

To only see apps from your team, from the **Team** dropdown, select your team.

![Select your team](images/use-team-ad.png)

Each square is an app. It shows the app name and the app type.

The color of each app shows you how high or low the technical debt is in that app.
Technical debt tells you how difficult or easy it is to change and maintain an app or module.

![Technical debt and agility color scale](images/use-debt-scale-ad.png)

Red means the app has high technical debt.

### Check the technical debt of the modules of the app

To get an overview all the modules of an app, double-click an app.  

![Overview of modules in an app](images/use-overview-app-ad.png)

Selecting a module highlights the dependencies of the module (if any).

![](images/use-module-dependencies-ad.png)

### Find and understand the causes of technical debt in an app

To go back and see all the app of your team, click **Back to Apps**.

![Back to Apps](images/use-back-to-apps-ad.png)

Select the app again. Make sure you don't double-click the app this time.

To see the causes of technical debt in the app, click the **Open app report** button in the side panel.

![Open app report](images/use-open-app-report-ad.png)

You can filter the report based on a specific app, module, category, when it was analyzed, the findings status, as well as specific users.

![Filters](images/use-filters-ad.png)

To see details about a code pattern that causes technical debt, click **Impact**. The **Impact** information details why a code pattern creates technical debt.

![Impact](images/use-report-impact-ad.png)

To check how to fix the code pattern, click **How to fix**. You can also use this information to understand the effort involved in fixing a code pattern.

![How to fix](images/use-report-fix-ad.png)

The **Findings** section displays all the occurrences of the code pattern. To see in which module and element each finding occurs, click the path icon.

![Findings](images/use-findings-ad.png)

After checking a finding, you can change it's state to one of the following:

* If you fix the finding, set the state to **Resolve as already fixed**. This lets other developers in your team know it's fixed. After the next synchronization, if you have solved the finding correctly, it disappears. Otherwise, the finding reverts to **Open**.

* If the finding is a false positive, set the state to **Resolve as false positive**. After the next synchronization, the finding is not counted towards the total technical debt score.

* If the finding isn't a false positive, set the state to **Resolve as won't fix** and detail the reason for not fixing it. After the next synchronization, the finding is not counted towards the total technical debt score.

* To temporarily remove the finding from the total debt calculation, set the state to **Remind me later (30 days)**. After the next synchronization, and during the next 30 days, the finding is not counted towards the total technical debt score.