---
title: Job
description: jenkinssuite Jenkins Suite Job Folder Create Delete Move Copy
categories:
  - jenkinssuite_en
tags:
  - jenkinssuite_en
---

This is the most used job in Jenkins. Features supported by Jenkins (?) Most of them are defined as Jobs.
As a result, this extension has the most features.
You can create a job, including creating a folder (this is also a job), and create/modify/delete/copy/move.
And it's not a feature of Jenkins, but you can do a scheduled build (within 2 hours).

## Job

### Generate Job Code (Ctrl + Alt + Insert)

> When you select Generate Job Code, you will be presented with a choice from the **Pipeline** / **FreeStyle** items, and select the type of job to create.

![JobTitle1](/images/job/job_01.png)

> When the auto-generated XML data is output to the Editor window, you can enter the required items and press Execute Job (Ctrl+K, F4) to reflect the settings

![JobTitle2](/images/job/job_02.png)

The auto-generated code is not supported by Jenkins, but will be customized as a feature of the extension.
{: .notice--warning}

### Create Folder

> When you select Create Folder, an InputBox appears, enter the name of the Folder you want to create, and a Folder is created

### Context Menu

![JobMenu](/images/job/job_03.png)

### Job Build

> If you select Job Build, the build will be performed immediately if there are no parameters, but if you need a parameter, you can enter the parameter through the InputBox.

Currently, only String parameters are supported.
{: .notice--warning}

### Config Job

> If you select Config Job, it looks up the XML and outputs it to the Editor window as shown in the image below.

* Just like View, you can change the job immediately by modifying the changes and updating it to the Jenkins server immediately
* After modifying the settings file (XML Data) in Jenkins, you can press Execute Job (Ctrl+K, F4) to reflect the settings.

![ConfigJob](/images/job/job_03.png)

### Rename Job

> If you select Rename on a job, you can change the name of the job by passing the name you want to change to the InputBox.

### Copy Job

> If you select Copy Job in a Job, you can copy the Job by passing the name you want to copy to the InputBox.

* If you select Copy from Folder, all sub-jobs are also copied.

### Move Job

> If you select Move a Job in a job, a list of views that can be moved will appear in the selection box, and if you select a View to move, the job will be moved to that View

### Delete Job

> If you select Delete in Job, it will be deleted immediately, so be careful when selecting.
