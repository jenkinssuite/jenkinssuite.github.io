---
title: Jenkins Suite Job
description: jenkinssuite Jenkins Suite Job Folder Create Delete Move Copy
categories:
  - jenkinssuite
tags:
  - jenkinssuite
---

Jenkins 에서 가장 많이 사용하는 Job 입니다. Jenkins에서 지원하는 기능(?)들은 대부분 Job으로 정의되어 있습니다.
그러다 보니 이 확장 프로그램에서도 가장 많은 기능이 적용되어 있습니다.
폴더 (이것 또한 Job) 생성을 비롯한 Job 및 생성/수정/삭제/복사/이동을 할 수 있습니다.
그리고 Jenkins 의 기능이 아니지만 예약 빌드 (2시간 이내)를 할 수 있습니다.

## Job 화면

### Generate Job Code (Ctrl + Alt + Insert)

> Generate Job Code 를 선택하면 **Pipeline** / **FreeStyle** 항목 중에서 선택하는 항목이 나오면 생성할 Job 의 종류를 선택합니다.

![JobTitle1](/images/job/job_01.png)

> Editor 창에 자동 생성된 XML 데이터가 출력되면 필요한 항목을 입력하고 Execute Job (Ctrl+K F4)를 눌러 설정을 반영할 수 있습니다

![JobTitle2](/images/job/job_02.png)

자동 생성된 코드는 Jenkins 에서 지원하는 것이 아닌 **확장 프로그램의 기능**으로 차후 커스터마이징을 추가할 예정입니다.
{: .notice--warning}

### Folder 생성

> 폴더 생성 (Create Folder)를 선택하면 InputBox 가 나타나고 생성할 Folder 의 이름을 입력하면 Folder 가 생성됩니다

### Context Menu

![JobMenu](/images/job/job_03.png)

### Job 빌드 (Build)

> Job을 빌드 (Build) 를 선택하면 파라미터가 없는 경우엔 바로 빌드를 수행하지만 만약 Parameter 가 필요하면 InputBox 를 통해서 파라미터를 입력할 수 있습니다.

현재는 String 파라미터만 지원 가능합니다.
{: .notice--warning}

### 설정 조회 (Config Job)

> 설정 조회 (Config Job)를 선택하면 하단의 이미지처럼 XML 를 조회해서 Editor 창에 출력한다.

* View 와 동일하게 Job 도 변경사항을 수정하고 바로 Jenkins 서버로 업데이트를 하면 바로 변경이 가능하다
* Jenkins 의 설정 파일 (XML Data)를 수정한 후에는 Execute Job (Ctrl+K F4)를 눌러 설정을 반영할 수 있습니다.

![ConfigJob](/images/job/job_03.png)

### Job 이름 변경 (Rename)

> Job 에서 이름 변경 (Rename)를 선택하면 InputBox 에 변경할 이름을 전달하면 Job의 이름을 변경할 수 있습니다.

### Job 복사 (Copy)

> Job 에서 Job 복사 (Copy)를 선택하면 InputBox 에 복사할 이름을 전달하면 Job을 복사할 수 있습니다.

* Folder 에서 복사를 선택하면 하위의 Job 들도 모두 복사된다.

### Job 이동 (Move)

> Job 에서 Job 이동 (Move)를 선택하면 현재 이동할 수 있는 View의 리스트가 선택박스로 나타나며 이동할 View를 선택하면 해당 View로 Job이 이동됩니다

### Job 삭제 (Delete)

> Job 에서 삭제 (Delete)를 선택하면 바로 삭제되므로 선택시에는 주의해야 합니다.
