---
title: Jenkins Suite Connection
description: Jenkins Suite settings connection
categories:
  - jenkinssuite
tags:
  - jenkinssuite
---

Jenkins Suite 를 사용하기 위해서는 Jenkins 서버의 설정을 해야 한다.

## Settings

* Connection 옆에 있는 Setting 아이콘을 누르면 우측 에디터 창에 Settings 화면이 나타난다.

![Settings](/images/settings/settings1_01.png)

* 설정 (Settings) 창에서 **Jenkinssuite: Servers** 하단에 있는 __Edit in settings.json__ 을 선택합니다.

![Servers](/images/settings/settings1_02.png)

* 에디터 창에 VS Code 의 환경설정 파일 settings.json 파일이 열리며 **"jenkinssuite.servers"** 의 키 값을 가지는 항목들이 새로 만들어지며 추가됩니다. 그러면 자신의 서버 환경에 맞는 값으로 변경합니다.

  * username: Jenkins 서버에 접속할 계정명
  * token: Jenkins Server에 로그인에 사용할 API Token [Token 생성 가이드](../../jenkins/jenkins-10-token/){: .btn .btn--info}
  * ssh: 서버에 접속하기 위한 SSH 설정
    * enabled: 사용 여부
    * address: SSH 서버 주소
    * port: SSH port number (default: 22)
    * username: SSH username
  * wstalk: Jenkins 서버의 WebSocket 서버의 설정 정보이며 Jenkins Server 의 별도 플러그인 설치 필요
  * git: Git 서버 URL

![settings_json](/images/settings/settings1_03.png)

* 설정을 맞게 수정을 한 후에 저장 (Ctrl + S)를 누른 후에 Connection 옆에 있는 Refresh 아이콘을 누르면 설정한 값이 반영됩니다.

![Refresh](/images/settings/settings1_04.png)

## Connect/Disconnect

### Connect

* Jenkins 서버에 접속하기 위해서는 접속할 서버에서 마우스 우측 버튼을 누르면 나오는 Context Menu 에서 Connect 를 선택합니다. (혹은 Alt+1 를 눌러 동일한 기능을 수행할 수 있습니다)

![Connect](/images/settings/connection1_01.png)

### Disconnect

* Jenkins 서버와 연결을 종료하기 위해서는 서버명에서 마우스 우측 버튼을 눌러 Disconnect 를 선택합니다.

### Connect SSH

* 설정에서 ssh를 **enabled: true** 를 하면 VS Code 내부의 SSH 프로그램을 사용하여 Jenkins 서버에 접속할 수 있습니다.

### Connect SSH with External

* 설정에서 ssh를 **enabled: true** 를 하면 외부 SSH 프로그램을 사용하여 Jenkins 서버에 접속할 수 있습니다.


## Admin 메뉴

> 로그인을 하면 추가적인 Admin 메뉴를 사용할 수 있습니다.

![Admin](/images/settings/connection2_01.png)

### Create User

> Jenkins 서버에 User/Admin/Guest 유저를 생성할 수 있습니다

![CreateUser](/images/settings/connection2_02.png)

### Set Default

> 자주 사용하는 서버가 있는 경우엔 설정해 두면 Sidebar 가 열릴 때 자동으로 설정된 서버로 자동 접속을 시도합니다.

### Change Executor

> Jenkins 서버에서 동시에 사용할 수 있는 Build 수를 변경할 수 있습니다.

![Executor](/images/settings/connection2_03.png)

### Create Secret Text / Create Username with password

> Jenkins 서버의 Manage Jenkins >> **Credentials** 에서 Global Credentails 에 추가할 수 있는 Secret Text / Username 를 생성할 수 있습니다.

![SecretText](/images/settings/connection2_04.png)