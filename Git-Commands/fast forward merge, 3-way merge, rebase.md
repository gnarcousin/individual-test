<h1> Fast-Foward-Merge, 3-Way-Merge, Rebase </h1>

<h2>fast forward merge</h2>

```bash
$ git merge 브랜치명
```

> - `Fast-Foward` = 순차적 커밋에 맞추어 병합을 처리하는 방식
> - 커밋 작업을 수행한 브랜치가 서로 다르나 **브랜치 경로가 1가지**인 경우 사용
>> - 작업한 브랜치의 **시작 커밋**을 원본 브랜치 **이후의 커밋**으로 가리킴
>>  - 원본에 추가할 내용이 없다는 가정 하에 **변경할 파일을 대체하는 것**과 같음

<h2>3-way merge</h2>

```bash
$ git merge 브랜치명 -edit
```

> - `3-way merge` : 주로 협업 시 사용하는 복잡한 병합 방법
> - 최신 커밋을 기준으로 브랜치 모양이 **여러 개로 갈라짐**
>> - `F-F` 알고리즘으로 병합이 불가능함
> -  **공통 조상 커밋을 기준**으로 각각 작업한 내용을 병합해줌
>> - 병합을 완료한 이후 **새로운 커밋(병합 커밋)을 생성**함
>>  - 병합 커밋은 부모 커밋이 2개라는 특징을 지님
> - 병합 메시지를 필수로 작성해야 함

<h2>rebase</h2>

```bash
$ git rebase 브랜치명
```

> - `rebase` : 공통 조상 커밋을 변경하는 병합 
>> - 두 브랜치를 **비교하지 않고 순차적으로** 커밋 병합)
> - `rebase`는 커밋의 위치를 재배치만 해주므로 병합된 브랜치의 **HEAD 포인터는 바뀌지 않음** 
>> - 이를 맞춰주기 위해 **브랜치 병합**을 해줘야 함
>>  - `F-F` 병합을 통해 **HEAD 포인터를 일치시키는 작업**까지 수행해야 최종 병합을 완성할 수 있음