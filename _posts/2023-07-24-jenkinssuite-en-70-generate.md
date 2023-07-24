---
title: Generate Custom Code
description: jenkinssuite Jenkins Suite Generate Custom Code Snippet XML Groovy Pipeline
categories:
  - jenkinssuite_en
tags:
  - jenkinssuite_en
---

In Jenkins, we have collected common or frequently used codes (XML, Pipeline) when creating jobs and displayed a list for ease of use so that it is easy to reuse. You can also register and use your own code.

For convenient use, enter **Generate Custom Job Code** in the Command Palette and use it easily through [**Ctrl + Shift + Insert**].
{: .notice--info}

## Generate Custom Code

> In the extension, you can see both the registered code and the code that you are registered with.

* The icon is separated so that it is easier for the user to see the registered code and the registered code in the extension.

![Custom1](/images/snippet/snippet_01.png)

### Register a custom code file

> If you select the settings icon in the Snippet Tree View, the Settings screen will be displayed in the editor window, and then find Snippet.custom-file and enter the full path of the file in your directory.

* The writing guide will be written separately.

![Custom2](/images/snippet/snippet_02.png)

### Creation Snippet Code

> After you find the code you want to use in the Snippet Tree View, select the + icon at the very end and it will be copied to the editor.

* In the image at the bottom, the Jenkins Language Mode is on the left and the XML Language Mode is on the right.

![Custom3](/images/snippet/snippet_03.png)

> After you're done, type **ExecuteQuick** or use the shortcut [Alt+Shift+Enter] in the Command Palette for quick execution.

* **ExecuteQuick** behaves differently depending on the _Language Mode_ (see the red part in the lower right corner of the image below).
  * **XML**: Create a Job or make changes [_Execute Job (Ctrl+K F4)_]
  * **Groovy**: Validate Jenkinsfile [_Validate Jenkinsfile (Ctrl+Alt+T)_]
