---
title: Jenkins Suite Jenkins Project
description: jenkinssuite Jenkins Suite Jenkins Project
categories:
  - jenkinssuite
tags:
  - jenkinssuite
---

대부분의 기능들이 별도의 사이드바에서 동작하던 것과 달리 이 기능은 사이드바의 전환없이 [Explorer (Ctrl+Shift+E)]에서 바로 배포하기를 원하는 경우에 사용할 수 있도록 만들었습니다. 그렇다 보니 많은 기능이 내포된 것이 아니라 개발 프로젝트에 종속되었기에 현재 프로젝트와 관련있는 몇개의 Job만 빨리 빌드할 수 있도록 구성되었습니다.

이 기능은 기본적으로 Jenkins Suite 의 서버 설정이 완료되어야만 사용할 수 있습니다. 즉 사용자 정보를 비롯한 Server 정보는 Jenkins Suite 설정을 공유합니다.
{: .notice--warning}

## Jenkins Project

![Explorer](/images/project/project_01.png)

* Explorer 뷰의 하단에 보면 Jenkins Project 가 있지만 처음엔 화면이 비어 있습니다. 그러면 타이틀 끝에 있는 Settings 아이콘을 선택하면 Editor 창에 .jenkinsrc.json 파일이 생성됩니다. 이 파일이 곧 Jenkins Project의 설정 파일입니다.

* 그러면 상단의 이미지와 비슷한 형태의 파일이 생성됩니다.
  * Local: 프로젝트에서 사용할 서버의 Jenkins Server 의 이름입니다. [Servers 이동](../jenkinssuite-30-connection){: .btn .btn--info}
  * applications: Job 의 URI 이며 배열 형태로 여러 개를 입력할 수 있습니다. URI 는 서버의 prefix 정보를 뺀 이후 입력하면 됩니다.

> 서버의 설정이 하단과 같은 경우라면 applications 의 정보는 다음과 같습니다.

* http://localhost:8080/jenkins/job/DemoJob1
* http://localhost:8080/jenkins/job/DemoJob

> 예: Jenkins Suite 의 서버 설정입니다

![settings_json](/images/settings/settings1_03.png)
