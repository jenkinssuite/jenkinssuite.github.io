---
title: Jenkins Suite Generate Custom Code
description: jenkinssuite Jenkins Suite Generate Custom Code Snippet XML Groovy Pipeline
categories:
  - jenkinssuite
tags:
  - jenkinssuite
---

Jenkins 에서는 Job 를 만들 때 공통적으로 혹은 자주 사용하는 코드 (XML, Pipeline)들을 모아 두고 사용하기 편리하도록 리스트를 표시해 재사용하기 용이하도록 하였습니다. 그리고 자신만의 코드도 등록하여 사용 할 수 있습니다.

편리하게 사용할 수 있도록 Command Palette 에서 **Generate Custom Job Code** 를 입력 [**Ctrl + Shift + Insert**] 를 통해서 쉽게 사용할 수 있도록 하였습니다.
{: .notice--info}

## Generate Custom Code

> 확장 프로그램에서 등록된 코드와 자신이 등록된 코드를 모두 볼 수 있습니다.

* 확장프로그램에서 등록된 코드와 사용자가 등록된 코드를 보기 쉽도록 아이콘을 구분하였습니다.

![Custom1](/images/snippet/snippet_01.png)

### Custom 코드 파일 등록

> Snippet Tree View 에 있는 설정아이콘을 선택하면 에디터 창에 Settings 화면이 출력된 후에 Snippet.custom-file 를 찾아 자신의 디렉토리에 있는 파일의 전체 경로를 입력한다.

* 작성 가이드는 따로 작성을 할 예정입니다.

![Custom2](/images/snippet/snippet_02.png)

### 코드 생성

> Snippet Tree View 에서 사용할 코드를 찾은 후에 가장 끝에 있는 + 아이콘을 선택하면 편집기로 복사됩니다.

* 하단의 이미지에서 좌측은 Jenkins Language Mode 이고 우측은 XML Language Mode 입니다.

![Custom3](/images/snippet/snippet_03.png)

> 작성을 완료한 후에 빠른 수행을 위해 Command Palette 에서 **ExecuteQuick** 를 입력 혹은 단축키 [Alt+Shift+Enter] 를 실행합니다.

* **ExecuteQuick** 은 _Language Mode_ (하기의 이미지 우측 하단 빨간 부분 참조)에 따라 다르게 동작을 합니다.
  * **XML**: Job 를 생성하거나 변경 수행 [_Execute Job (Ctrl+K F4)_]
  * **Groovy**: Jenkinsfile 의 유효성 검사 수행 [_Validate Jenkinsfile (Ctrl+Alt+T)_]
