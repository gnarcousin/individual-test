<h1> branch, checkout, switch </h1>

<h2> branch </h2>

```git
$ git branch # 브랜치 목록 출력

$ git branch 브랜치명 [커밋ID]
```

> - `branch` 명령어 뒤에 브랜치 이름을 인자값으로 추가해 **브랜치 생성**
> - 기준이 될 커밋 ID 지정 안할 시 현재 `HEAD` 포인터를 기준으로 새로운 브랜치를 생성함

```git
$ git branch -d

$ git branch -D #브랜치 강제 삭제
```

> - `-d` 옵션은 **SA가 깨끗할 때만** 삭제를 허용함
> - `-d` 옵션은 **병합되지 않은 브랜치 삭제 불가능**

<h2> checkout </h2>

```git
$ git checkout 브랜치명

$ git checkout -b 브랜치명 #브랜치를 생성하고 자동 이동

$ git checkout 커밋해시키 #브랜치 이름 대신 커밋 해시키를 사용해 이동

$ git checkout HEAD~x #HEAD를 기준으로 x단계 전의 커밋 상태로 이동
```

> - 브랜치 간의 **이동을 수행함**
> - 브랜치명 대신 대시`-`를 사용하면 **바로 이전 브랜치로** 복귀함
> - 다른 브랜치에서 작업하기 위해서는 브랜치를 변경해 **WD를 재설정** 해줘야 함
>> - WD에 **커밋되지 않은 내용이 존재하면 브랜치 변경이 불가능**

<h2> switch </h2>

```git
$ git switch 브랜치명

$ git switch -c 브랜치명 #브랜치 생성과 동시에 브랜치 전환
```

> - `switch` 명령어 옆의 **특정 브랜치로 전환함**
