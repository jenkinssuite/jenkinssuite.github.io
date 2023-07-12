---
title: Jenkins Suite View
description: jenkinssuite Jenkins Suite View
categories:
  - jenkinssuite
tags:
  - jenkinssuite
---

Jenkins 에 접속하면 처음 나오는 Dashboard (메인 페이지) 에서 볼 수 있는 View 의 리스트와 동일한 목록입니다. View 를 생성/수정 혹은 설정을 조회하거나 변경할 수 있습니다.

![View](/images/view/view_01.png)

## View

### Create View

> Views 옆에 있는 + (Create View)를 누르면 InputBox 가 보이고 그 InputBox에 생성할 View 의 이름을 입력합니다.

![CreateView](/images/view/view_02.png)

### Get Config View

> 기존 *All* View 혹은 새로 생성한 View에서 마우스 우측 버튼을 누르면 해당 View 의 설정를 조회할 수 있습니다.

* columns 의 순서와 includeRegex 를 간단하게 수정할 수 있다.
* Jenkins 의 설정 파일 (XML Data)를 수정한 후에는 Execute View (Ctrl+K F3)를 눌러 설정을 반영할 수 있다.

![GetConfig](/images/view/view_04_01.png)

<br />

![Jenkins_GetConfig](/images/view/view_04_02.png)

### Rename View

> Default view 가 아닌 경우에는 View 의 이름을 변경할 수 있다.
