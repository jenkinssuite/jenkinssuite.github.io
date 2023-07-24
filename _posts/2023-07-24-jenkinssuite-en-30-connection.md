---
title: Connection
description: jenkinssuite Jenkins Suite Settings connection
categories:
  - jenkinssuite_en
tags:
  - jenkinssuite_en
---

To use Jenkins Suite, you need to configure the Jenkins server.

## Settings

* If you click the Setting icon next to Connection, the Settings screen appears in the right editor window.

![Settings](/images/settings/settings1_01.png)

* In the Settings window, select __Edit in settings.json__ at the bottom of Jenkinssuite: Servers.

![Servers](/images/settings/settings1_02.png)

* The VS Code configuration file settings.json file opens in the editor window, and new entries with the key value of "jenkinssuite.servers" are created and added. Then change it to a value that is appropriate for your server environment.

  * username: The name of the account to connect to the Jenkins server.
  * token: API token to use to log in to Jenkins Server [TokenCreation](../../jenkins_en/jenkins-en-10-token/){: .btn .btn--info}
  * ssh: Setting up SSH to connect to the server
    * enabled: Whether to use it
    * address: SSH server address
    * port: SSH port number (default: 22)
    * username: SSH username
  * wstalk: This is the setting information of the WebSocket server of the Jenkins server, and a separate plug-in installation of the Jenkins server is required.
  * git: URL of the Git Server

![settings_json](/images/settings/settings1_03.png)

* After modifying the settings accordingly, press Save (Ctrl + S) and then click the Refresh icon next to Connection to reflect the set values.

![Refresh](/images/settings/settings1_04.png)

## Connect/Disconnect

### Connect

* To connect to the Jenkins server, select Connect from the Context Menu that appears when you press the right mouse button on the server to be connected. (Alternatively, you can press Alt+1 to perform the same function.)

![Connect](/images/settings/connection1_01.png)

### Disconnect

* To terminate the connection with the Jenkins server, press the right mouse button in the server name and select Disconnect.

### Connect SSH

* If you enable ssh in your settings, you can use the SSH program inside VS Code to connect to the Jenkins server.

### Connect SSH with External

* If you set ssh to __enabled: true__ in the settings, you can use an external SSH program to connect to the Jenkins server.

## Admin Menu

> Once you are logged in, you can use the additional Admin menu.

![Admin](/images/settings/connection2_01.png)

### Create User

> You can create User/Admin/Guest users on the Jenkins server

![CreateUser](/images/settings/connection2_02.png)

### Set Default

> If you have a server that you use frequently, set it up and it will automatically try to connect to the server that is set automatically when the Sidebar is opened.

### Change Executor

> You can change the number of builds that can be used on a Jenkins server at the same time.

![Executor](/images/settings/connection2_03.png)

### Create Secret Text / Create Username with password

> You can create a Secret Text / Username that can be added to Global Credentails from the Manage Jenkins >> Credentials on the Jenkins server.

![SecretText](/images/settings/connection2_04.png)
