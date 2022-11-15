<h1> clone, push, pull, fetch, merge </h1>

<h2> clone </h2>

```git
$ git clone 원격저장소URL
```

> - 초기화 `init` 명령어를 제외한 원격 서버 **연결에 필요한 추가 설정을 자동으로 수행**
> - 연결 설정을 마친 뒤 서버 내의 **모든 커밋 이력들**을 한번에 내려받음

<pre>
원격 저장소 정보 확인 명령어
<code> $ git remote -v </code>
</pre>

<h2> push </h2>

```git
$ git push
```

> - 로컬 저장소 내의 커밋된 파일들을 **원격 저장소로 업로드**함

<h2> pull </h2>

```git
$ git pull
```

> - `clone` 이후 원격 저장소의 **갱신된 내용**을 추가로 내려받음
> - 로컬 저장소보다 **최신인 원격 저장소의 커밋 정보**를 내려받음
>> - pull 명령어의 주기적인 사용으로 로컬 저장소를 최신 정보로 유지할 수 있음

<h2> fetch </h2>

```git
$ git fetch 원격저장소URL
```

> - 임시 브랜치를 생성해 원격 저장소의 최신 커밋들을 **수동으로 내려받음**
> - 병합을 자동으로 해주지 않음

<h2> merge </h2>

```git
$ git merge 원격저장소별칭/브랜치명
```

> - `fetch`로 내려받은 커밋들을 **병합**해줌
> - `fetch`로 내려받은 `remote branch`들도 병합
