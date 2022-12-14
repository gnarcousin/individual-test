<h1> Reset, Revert </h1>

<h2> Reset </h2>

```bash
$ git reset 옵션 커밋ID
```

> - `reset` = 지정된 커밋 코드로 되돌아감
>> - 특정 커밋의 **해시 값 상태로 모든 코드를 복구**
>> - `soft`, `mixed`, `hard` 등의 다양한 옵션 존재
> - 커밋 ID 이외에도 *파일이름, HEAD 포인터*를 기준으로도 실행 가능
> - 커밋, 작업, 병합도 마찬가지로 취소 가능함

<h2> Revert </h2>

```bash
$ git revert 커밋 ID
```

> - `revert` = **기존 커밋을 남겨두고** 삭제를 위한 새로운 커밋 생성
> - **한번에 하나의 커밋만 취소 가능**
> - 병합도 선택 취소 가 가능함 `--mainline` 옵션 사용
> - `reset`은 커밋을 삭제하기 때문에 **협업**에서는 커밋을 유지하는 `revert`가 더 유용함
