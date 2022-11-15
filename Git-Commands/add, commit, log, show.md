<h1> Commands add, commit, log, show </h1>

<h2> 깃의 영역 구조 </h2>

![285623](https://user-images.githubusercontent.com/107753319/201808850-2ea79505-91fe-418b-9311-afc9335b5505.png)

> - **Working Directory(WD)** = 현재 작업 중인 공간
> - **Staging Area (SA)** = 임시 저장 공간
> - **Repository** = 저장소

<h2> add </h2>

```git
$ git add 파일명

$ git add . # 폴더와 폴더 내 전체 파일을 모두 등록함
```
> - WD의 파일을 SA에 추가
> - 파일을 **tracked 상태로 변경**함
>> - 빈 폴더는 SA에 추가할 수 없음

<h2> commit </h2>

<h6> 커밋 </h6>

```git
$ git commit

$ git commit -help #커밋 옵션 표시
```
> - commit 명령어는 **독립적인 사용이 가능**함
> - 여러 옵션을 같이 사용 가능
> - SA 내의 파일만 커밋할 수 있음 (tracked 상태여야 함)
> - 파일의 변경 내용과 기록을 영구적으로 깃 저장소에 저장함

<h6> 커밋 메시지 </h6>

```git
$ git commit -m '메시지'

$ git commit -am '메시지' # 파일 등록과 커밋을 한번에 해줌
```

> - 깃은 커밋을 통해 **파일의 차이점**을 기록함
> - 기록된 파일 객체들을 구별하기 위해 모든 커밋은 커밋 메시지를 작성해야 함
> - **커밋 메시지** = 커밋을 구별하기 위해 작성하는 설명
> - `-a` 옵션은 커밋 이전에 자동으로 모든 파일을 등록하는 과정을 미리 수행함

<h2> log </h2>

```git
$ git log
```

> - **커밋 기록**을 확인
> - `git config`를 통해 설정한 파일들을 표시하고 커밋 기록들을 출력해줌

<h2> show </h2>

```git
$ git show
```

> - `log`에서 표시한 정보에 더해 파일의 변화 `patch`도 함께 표시함
