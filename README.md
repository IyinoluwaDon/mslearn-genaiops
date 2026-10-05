
## GitHub Use & Purpose

Microsoft Learning is using GitHub to publish the lab steps and lab scripts for courses that cover cloud services like Azure. Using GitHub allows the course’s authors and MCTs to keep the lab content current with Azure platform changes. Using GitHub allows the MCTs to provide feedback and suggestions for lab changes, and then the course authors can update lab steps and scripts quickly and relatively easily.

> When you prepare to teach these courses, you should ensure that you are using the latest lab steps and scripts by downloading the appropriate files from GitHub. GitHub should not be used to discuss technical content in the course, or how to prep. It should only be used to address changes in the labs.

> As an alternative to pointing students directly to the GitHub repository, you can point students to the GitHub Pages website to view the lab instructions. The URL for the GitHub Pages website can be found at the top of the repository.

To address general comments about the course and demos, or how to prepare for a course delivery, please use the existing MCT forums.

## Additional Resources

A user guide has been provided for MCTs who are new to GitHub. It provides steps for connecting to GitHub, downloading and printing course materials, updating the scripts that students use in labs, and explaining how you can help ensure that this course’s content remains current.

<https://microsoftlearning.github.io/MCT-User-Guide/>


---
title: GenAI Operations Exercises  
permalink: index.html
layout: home
---

# GenAI Operations (GenAIOps) Workload Labs

The following hands-on exercises provide practical experience with GenAI Operations patterns and practices. You'll learn to deploy infrastructure, manage prompts, implement evaluation workflows, and monitor production GenAI applications using Microsoft Foundry and Azure services.

> **Note**: To complete the exercises, you'll need an Azure subscription with sufficient permissions and quota to provision Azure AI services and deploy Microsoft Foundry workspaces. If you don't have an Azure subscription, you can sign up for an [Azure account](https://azure.microsoft.com/free) with free credits for new users.

## Quickstart exercises

{% assign labs = site.pages | where_exp:"page", "page.url contains '/docs'" %}
{% for activity in labs  %}
<hr>
### [{{ activity.lab.title }}]({{ site.github.url }}{{ activity.url }})

{{activity.lab.description}}

{% endfor %}

> **Note**: While you can complete these exercises on their own, they're designed to complement modules on [Microsoft Learn](https://learn.microsoft.com/training/paths/operationalize-gen-ai-apps/); in which you'll find a deeper dive into some of the underlying concepts on which these exercises are based.
