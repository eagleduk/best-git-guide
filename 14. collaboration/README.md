## collaboration

### centralized workflow

- 중앙 집중형 워크플로우
- 메인 `branch`(`master` 또는 `main`)로 작업하는 협업
- 미완성된 작업은 `push` 하면 다른 작업자 전체가 미완성인 작업을 가지게 된다.
- 매번 작업내용을 `merge`하는 작업이 필요하다.

### Feature Branch

- 메인 `branch`(`master` 또는 `main`)에서 절대 작업을 하지 않는다.
- 본인의 작업에 대하여 협업이 필요한 경우, `merge` 하지 않고도 해당 `branch`를 내려받아 협업이 가능하다.
- 작업 `branch`에서 완료된 기능을 메인 브런치(`master` 또는 `main`)에 `merge` 할 때 승인 및 테스트 통과 이후 관리자가 병합한다.
- 메인 `branch`(`master` 또는 `main`)에는 배포 및 서비스 가능한 상태를 유지한다.
- 필요없는 기능(`branch`) 는 병합되지 않거나 무시가 가능하다.
- 작업 `branch` 기능이 완료되고, 메인 `branch`에 병합되면 작업 `branch`는 삭제한다.

### Merging Feature Branches

1. 개인적인 `branch` 통합 순서를 협의 하여 메인 `branch`에 통합
2. `Pull Request(PR)`

### Pull Request

- 공동 작업자들에게 검토를 요청하고 `merge`를 **승인** 또는 **반려**를 요청하는 작업
- 공동 작업자가 아닐 경우에는 `fork` 및 `Clone` 작업이 후 `Pull Request`를 요청한다.
- `Pull Request`시 `conflict`가 발생하면
  1. 저장소의 페이지에서 `merge`한다.
  2. 로컬의 저장소에서 `merge` 작업 이후 `push`한다.

### branch protect

### Fork

- `Github`기능이지만 원격 저장소에서는 같은 이름으로 기능을 제공한다.(BitBucket, Gitlab)
- 공동 작업자가 아닌 저장소를 본인의 계정에 복사하는것
- 개인 저장소에 복사하는 것이기 때문에 자유롭게 접근하고 작업이 가능하다.
- 공동 작업자 권한이 없더라도 작업이 가능하다.
- 원본 저장소(`upstream`)과 병합을 하려면 `Pull Request`를 통하여 원본 작업자에게 요청하여 병합한다.
- 원본 저장소(`upstream`)에 병합 권한은 없지만 `pull`은 가능하다.

  - `pull`기능을 수행하려면 `remote`연결이 필요하다.

    ```shell
    git remote add <original-repositry-name> <original-repository-url>
    ```
