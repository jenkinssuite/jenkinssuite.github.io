---
title: Jenkins Suite Layout
description: Jenkins Suite Layout
categories:
  - jenkinssuite
tags:
  - jenkinssuite
---

Jenkins Suite 를 설치하고 나면 좌측 Activity Bar 에 새로운 Jenkins 아이콘을 볼 수 있습니다.
그것을 클릭하면 Jenkins Suite 의 SideBar는 총 7개의 TreeView로 구성되어 있으며 다음과 같습니다.

## 화면 구성

### Connection

> 접속할 수 있는 서버의 목록과 접속 상태 등을 확인할 수 있습니다. 상단의 설정 아이콘을 선택하면 쉽게 서버의 설정 추가/변경할 수 있습니다.

  - Connect: Jenkins 서버 연결
  - Disconnect: Jenkins 서버 종료
  - Connect SSH: SSH 서버 연결
  - Conenct SSH with External: 외부 프로그램을 이용한 SSH 서버 연결
  - Create User: Jenkins User 생성
  - Set Default: 기본 연결로 설정
  - Change Executor: 한 번에 최대 실행할 수 있는 빌드 개수 변경
  - Create Secret Text: Secret Text 생성 [Credentials]
  - Create Username with password: Secret Text 생성 [Credentials]
![Connection](/images/settings/settings1_01.png){: .align-center}

### Views

> Jenkins 서버의 전체 View 를 볼 수 있으며 생성/전환할 수 있습니다.

  - Get Config View: View 의 설정 정보 (XML)를 에디터 창에 출력
  - Rename View: View 의 이름을 변경. 단 Default View 로 설정된 View 의 이름은 변경 불가
![Views](/images/settings/settings1_02.png){: .align-center}

### Jobs

> 해당 View에 존재하는 Job (Folder 포함) 를 보거나 빌드/생성/수정할 수 있습니다.

  - Build: Job 빌드
  - Get Config Job: Job 의 설정 정보 (XML)를 에디터 창에 출력
  - Open External Browser: 외부 브라우저를 이용해 현재 Job 화면으로 이동
  - Add Reservation: 빌드 예약 (3 ~ 120분 사이로 설정 가능)
  - Rename: Job 명 변경
  - Copy: Job 복사
  - Move: Job 이동
  - Delete: Job 삭제
  - Disabled: Job 을 Disable 상태로 변경
![Jobs](/images/settings/settings1_03.png){: .align-center}

### Builds of Job

> Jobs TreeView에서 선택한 해당 Job의 빌드 기록을 볼 수 있으며 Console (로그) 화면을 열 수 있습니다.

  - Get Job Log: 에디터창에 현재 빌드 결과를 출력
  - Open With Browser Log: 외부 브라우저를 통해 빌드 결과 페이지로 이동
![Builds of Job](/images/settings/settings1_04.png){: .align-center}

### Reservation

> 이 기능은 Jenkins Server 에서 실행되는 것이 아닌 VS Code 에서 구현한 기능으로 최소 3 ~ 120분 으로 설정할 수 있으며 설정한 시간에 빌드를 수행하는 빌드 예약/취소를 할 수 있습니다.

단 이 기능은 Jenkins 서버를 통해 동작하는 기능이 아니므로 VS Code 가 종료시에는 동작하지 않습니다.
{: .notice--warning}

![Reservation](/images/settings/settings1_05.png){: .align-center}

### Notify

> Jenkins plugin WSTalk [WsTalk로 이동](https://github.com/utocode/wstalk/releases/){: .btn .btn--info}를 다운로드 받아서 설치를 하면 사용할 수 있는 기능으로 Jenkins 에서 빌드를 하면 WebSocket 를 이용해 Notification 를 받을 수 있습니다.

### Snippet

> 많이 사용하는 Jenkins 의 Job 생성 파일 (XML), Groovy, Jenkinsfile 등을 저장해 두고 사용할 수 있습니다.

  - Generate Code From Snippet: Jenkins 의 Job 생성 파일 (XML), Groovy, Jenkinsfile 가져오기

![Snippet](/images/settings/settings1_07.png){: .align-center}
