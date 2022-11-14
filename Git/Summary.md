<h1>Git</h1>

<h2>Git이란?</h2>

> - 대표적인 **분산형** 버전 관리 프로그램
> - **원격 저장소와 로컬 저장소**로 이루어져 소스 코드가 각각 관리됨
>> + 오프라인으로 로컬 저장소에서 작업한 것을 온라인으로 원격 저장소와 동기화시킬 수 있음
> - 코드의 **배포나 수정 · 병합**이 자유로움 

<h2>특징</h2>

> - **백업 기능**이 존재함
>> + 로컬 저장소를 통해 **독립적인 소스의 버전 관리가 가능**
> - **협업에 특화**되어 있음
>> - 다수의 개발자와 코드를 공유 · 협업함에 있어 다른 VCS들보다 뛰어남

<h2>Git의 협업 특징</h2>

> - **코드 공유**
> 
>   - 네트워크를 이용해 온라인에서 다른 개발자들과 더 쉽게 코드를 공유 가능함
>   
> - **책임과 기록**  
> 
>   - 깃은 커밋으로 모든 코드의 수정 이력을 기록하는데, **커밋으로 저장된 원본 객체는 수정할 수 없어** 신중하게 작업해야 함
> 
> - **원격 공유**
> 
>   - 깃은 원격 저장소가 중앙 서버의 역할을 함
>   - 개발자들은 자신의 코드를 저장소에 `push`해 동기화하고 다른 개발자의 소스를 `pull` / `fetch`를 통해 내려받음
>
> - **병합**
> 
>   - 깃은 하나의 소스 코드에서 **여러 브랜치로 분기를 나눠 독립적으로 관리가 가능**함
>   - 독립적으로 구현된 소스들을 필요에 따라 병합하기도 하는데, 깃은 이 작업을 자동으로 수행하게 도와줌
>   - 이를 통해 소스 코드의 병합을 수동 병합에 비해 상대적으로 쉽게 할 수 있음
>   
> - **공개**
> 
>   - 깃은 원격 저장소를 통해 개발 중인 코드를 **외부로 공개 가능**
>   - 이를 통해 **외부 개발자와 협업이 가능함**
>   - 외부 개발자는 원격 저장소를 `fork`해 수정한 후 `pull request`로 병합 제안을 하는 식으로 개발자를 도울 수 있음