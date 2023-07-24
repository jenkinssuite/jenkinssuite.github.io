---
title: Jenkins Project
description: jenkinssuite Jenkins Suite Jenkins Project
categories:
  - jenkinssuite_en
tags:
  - jenkinssuite_en
---

Unlike most features that work in a separate sidebar, this feature is designed to be used when you want to deploy directly from Explorer (Ctrl+Shift+E) without switching sidebars. As a result, many functions are not implied, but are dependent on the development project, so only a few jobs related to the current project can be built quickly.

By default, this feature is only available after the server setup in Jenkins Suite is complete. In other words, server information, including user information, shares Jenkins Suite settings.
{: .notice--warning}

## Jenkins Project

![Explorer](/images/project/project_01.png)

* At the bottom of the Explorer view, you can see the Jenkins Project, but the screen is blank at first. Then, selecting the Settings icon at the end of the title will create a .jenkinsrc.json file in the Editor window. This is the configuration file for the Jenkins Project.

* This will create a file similar to the image above.
  * Local: The name of the Jenkins Server server to be used in the project. [Servers](../jenkinssuite-en-30-connection){: .btn .btn--info}
  * Applications: This is the URI of the Job and allows you to enter multiple of them in the form of an array. The URI can be entered after subtracting the server's prefix information.

> If the server's settings are the same as below, the information in applications is as follows.

* http://localhost:8080/jenkins/job/DemoJob1
* http://localhost:8080/jenkins/job/DemoJob

> Example: Server settings for Jenkins Suite

![settings_json](/images/settings/settings1_03.png)
