---
title: Jenkins Suite Reservation
description: jenkinssuite Jenkins Suite Reservation
categories:
  - jenkinssuite
tags:
  - jenkinssuite
---

Jenkins 를 사용하면서 (설정을 변경하지 않고) 10분 혹은 30분 후에 한 번만 빌드를 했으면 하는 아쉬움이 있어서 만들었습니다.
(그 사이 누군가 플러그인 개발을 완료했는 지도 모르겠지만^^;)

이 기능은 Jenkins 서버의 기능이 아닌 확장 프로그램에서 스케쥴링하는 기능이므로 VS Code 를 종료시에는 실행되지 않습니다.
{: .notice--warning}

## Reservation

### Add Reservation

> 예약 빌드 (Add Reservation)를 하려면 Job Tree View 화면에서 원하는 Job 를 선택하고 마우스 우측 버튼을 누른 후에 Add Reservation 를 선택합니다.

* 예약 빌드는 최소 3분 ~ 최대 120분 (2시간)까지 설정할 수 있습니다.

![reservation1](/images/reservation/reservation_01.png)

> 에약 빌드를 하게 되면 Reservation Tree View 에서 확인하실 수 있습니다. 등록되는 시간이 아닌 실행되는 순서로 표시됩니다.

![reservation2](/images/reservation/reservation_02.png)

### Cancel Reservation

> 예약을 취소하려면 Reservation Tree View 에서 취소할 Job를 찾은 후에 가장 마지막에 있는 X 아이콘을 선택합니다.
