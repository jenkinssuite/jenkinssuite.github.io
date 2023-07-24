---
title: Layout
description: jenkinssuite Jenkins Suite Layout
categories:
  - jenkinssuite_en
tags:
  - jenkinssuite_en
---

Once you've installed Jenkins Suite, you'll see a new Jenkins icon in the Activity Bar on the left.
If you click on it, you will see that the SideBar in Jenkins Suite consists of a total of 7 TreeViews, and they look like this:

## Layout

### Connection

> You can check the list of servers that can be connected and the connection status.
If you select the settings icon at the top, you can easily add/change the server's settings.

* Connect: Jenkins Connection
* Disconnect: Jenkins Disconnection
* Connect SSH: SSH Server Connection
* Conenct SSH with External: Connecting to an SSH server using an external program
* Create User: Jenkins User Creation
* Set Default: Set as the default connection
* Change Executor: Change the maximum number of builds that can run at a time
* Create Secret Text: Secret Text Creation [Credentials]
* Create Username with password: Secret Text Creation [Credentials]
![Connection](/images/layout/layout_01.png){: .align-center}

### Views

> You can see the entire View of the Jenkins server and can create/switch between them.

* Get Config View: View settings information (XML) output to the editor window
* Rename View: Change the name of the View. However, the name of the View set to Default View cannot be changed.
![Views](/images/layout/layout_02.png){: .align-center}

### Jobs

> You can view, build, create, and modify jobs (including folders) that exist in that View.

* Build: Job Build
* Get Config Job: Output the job setting information (XML) to the editor window
* Open External Browser: Use an external browser to navigate to the current job screen
* Add Reservation: Schedule a build (can be set between 3 ~ 120 minutes)
* Rename: Rename Job
* Copy: Copy Job
* Move: Move Job
* Delete: Delete Job
* Disabled / Enabled: Disabled / Enabled Job
![Jobs](/images/layout/layout_03.png){: .align-center}

### Builds of Job

> You can view the build history of the selected job in the Jobs TreeView, and you can open the Console (log) screen.

* Get Job Log: Print the current build result in the editor window
* Open With Browser Log: Go to the build results page via an external browser
![Builds of Job](/images/layout/layout_04.png){: .align-center}

### Reservation

> This feature is implemented in VS Code, not running on Jenkins Server, and can be set to a minimum of 3 ~ 120 minutes, and you can schedule/cancel a build that performs the build at a set time.

However, this feature does not work through the Jenkins server, so it does not work when VS Code is shut down.
{: .notice--warning}

![Reservation](/images/layout/layout_05.png){: .align-center}

### Notify

> Jenkins plugin WSTalk [Go to WsTalk](https://github.com/utocode/wstalk/releases/){: .btn .btn--info} is a function that can be used by downloading and installing, and if you build it in Jenkins, you can receive notification using WebSocket.

### Snippet

> You can save and use Jenkins' job creation file (XML), Groovy, Jenkinsfile, etc., which are commonly used.

* Generate Code From Snippet: Get Jenkins' Job Creation File (XML), Groovy, Jenkinsfile

![Snippet](/images/layout/layout_07.png){: .align-center}
