---
title: Jenkins Token Creation
description: Jenkins Token Creation
categories:
  - jenkins_en
tags:
  - jenkins_en
---

First of all, in order to access the Jenkins server from Jenkins Suite, you need to obtain an API token for the Jenkins server. <br />
In this case, we will proceed with the premise that there is a Jenkins server (e.g. <http://192.168.0.1:8080/jenkins>) and the account is admin. <br />
If you have already received it or know about it, you can proceed to the next one.

## Procedure

### Login

+ Log in and connect to the Jenkins server.
+ On the main screen, select People from the left menu. <br />
![Main](/images/jenkins/jenkins1.png){: .align-center}

+ Select your own account. <br />
![Account](/images/jenkins/jenkins2.png){: .align-center}

+ Select Configure from the menu on the left. <br />
![Configure](/images/jenkins/jenkins3.png)

### API Token Generate

+ When the Configure screen appears, select the API Token >> ADD NEW TOKEN BUTTON. <br />
![Token](/images/jenkins/jenkins4.png)

+ Select the Generate button. <br />
![Generate](/images/jenkins/jenkins5.png)

+ After copying the generated Token value, save it well so that you do not forget it. This token is used by **Plug-in Settings**[Go to Settings](/jenkinssuite/jenkinssuite-30-connection/#settings){: .btn .btn--info}
![Token](/images/jenkins/jenkins6.png)
