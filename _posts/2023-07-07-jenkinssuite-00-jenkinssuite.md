---
title: Jenkins Suite
description: Jenkins Suite 한글 가이드
categories:
  - jenkinssuite
tags:
  - jenkinssuite
---

Jenkins Suite 에 대한 가이드를 제공합니다. <br />
이 프로그램은 [Visual Studio Code](https://code.visualstudio.com/)의 Extension 프로그램이지만 [Jenkins](https://www.jenkins.io/) 서버를 필요로 합니다. 그렇기 때문에 Jenkins 가 설치된 서버 환경이나 로컬에 직접 설치해야만 사용할 수 있습니다. <br />
VSCode 에서 편리하게 Jenkins 의 기능을 사용 (빌드)하고자 하는 매우 단순한 생각으로 개발되었기 때문에 주요한 기능들은 마우스 대신 키보드를 사용하시면 편리하게 사용하실 수 있습니다.

기본적으로 다음의 프로그램이 먼저 설치되어 있어야 합니다.

## Prerequisites

1. Jenkins [다운로드](https://www.jenkins.io/download/){: .btn .btn--info}
2. Visual Studio Code [다운로드](https://code.visualstudio.com/Download){: .btn .btn--info}
3. Jenkins Suite [다운로드](https://marketplace.visualstudio.com/items?itemName=utocode.jenkinssuite){: .btn .btn--info}

다음의 Jenkins 플러그인은 필수는 아니지만 설치를 권장합니다.

## Optional Install [Recommend]

- JobDSL [https://plugins.jenkins.io/job-dsl/](https://plugins.jenkins.io/job-dsl/)
- categorized-view [https://plugins.jenkins.io/categorized-view/](https://plugins.jenkins.io/categorized-view/)
- WsTalk [https://github.com/utocode/wstalk/releases/](https://github.com/utocode/wstalk/releases/)

WsTalk은 수동 설치만 가능합니다.
{: .notice--warning}

<br />

## 목차

- [Jenkins 서버의 Token 생성](../../jenkins/jenkins-10-token/)
- [화면 구성](../jenkinssuite-20-layout/)
- [설정 / 접속](../jenkinssuite-30-connection)
- [View 전환 및 생성](../jenkinssuite-40-view)
- [Job 생성 및 수정, 실행](../jenkinssuite-50-job)
- [Job 예약](../jenkinssuite-60-reservation)
- [Generate Code](../jenkinssuite-70-generate)

이 문서는 Jenkins 및 VS Code가 설치되어 있다는 가정하에 작성되었습니다.
{: .notice--success}
