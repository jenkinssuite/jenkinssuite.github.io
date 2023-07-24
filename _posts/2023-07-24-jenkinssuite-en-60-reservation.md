---
title: Reservation
description: jenkinssuite Jenkins Suite Reservation Schedule Job
categories:
  - jenkinssuite_en
tags:
  - jenkinssuite_en
---

I made it because I was using Jenkins and wished I had only built once after 10 or 30 minutes (without changing the settings).

This feature is a feature that is scheduled by the extension, not a feature of the Jenkins server, so it won't run when VS Code is closed.
{: .notice--warning}

## Reservation

### Add Reservation

> To make an Add Reservation, select the desired Job on the Job Tree View screen, press the right mouse button, and then select Add Reservation.

* Scheduled builds can be set from a minimum of 3 minutes ~ a maximum of 120 minutes (2 hours).

![reservation1](/images/reservation/reservation_01.png)

> Once you have a reserved build, you can check it in the Reservation Tree View. It is displayed in the order in which it is executed, not when it is registered.

![reservation2](/images/reservation/reservation_02.png)

### Cancel Reservation

> To cancel a reservation, find the job you want to cancel in the Reservation Tree View and select the X icon at the end.
