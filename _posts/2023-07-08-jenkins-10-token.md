---
title: Jenkins 서버의 Token 생성
description: Jenkins 서버의 Token 생성
categories:
  - jenkins
tags:
  - jenkins
  - token
---

우선 Jenkins Suite에서 Jenkins 서버에 접근하기 위해서는 Jenkins 서버의 API 토큰을 발급받아야 합니다. <br />
여기서는 Jenkins 서버 (예: http://192.168.0.1:8080/jenkins)가 있고 계정은 admin 이라는 전제로 설명을 진행하도록 하겠습니다. <br />
이미 발급받았거나 아시는 분들은 다음으로 진행하셔도 무방합니다.

## 절차

### 로그인

+ Jenkins 서버에 로그인하고 접속합니다.
+ 메인 화면에서 좌측 메뉴의 People 를 선택합니다. <br />
![메인화면](/images/jenkins/jenkins1.png){: .align-center}

+ 자신의 계정을 선택합니다. <br />
![계정](/images/jenkins/jenkins2.png){: .align-center}

+ 좌측 메뉴에서 Configure 를 선택합니다.  <br />
![Configure](/images/jenkins/jenkins3.png)

### API Token Generate

+ Configure 화면이 나오면 API Token >> ADD NEW TOKEN 버튼을 선택합니다.<br />
![Token](/images/jenkins/jenkins4.png)

+ Generate 버튼을 선택합니다. <br />
![Generate](/images/jenkins/jenkins5.png)

+ 생성된 Token 값을 복사한 후에 잊어버리지 않도록 잘 저장합니다. 이 Token은 **플러그인 설정**[설정으로 이동](/jenkinssuite/jenkinssuite-30-connection/#settings){: .btn .btn--info} 에서 사용합니다.
![Token](/images/jenkins/jenkins6.png)
