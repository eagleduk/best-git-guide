## rebase

```shell
git rebase <branch-name>
```

- 두개의 `branch`를 병합하는 기능
- `merge` 대신 사용하는 병합
- `git` 이력을 지우는 작업
- `branch`에 올려진 `commit`을 각각 새 `commit`으로 생성
- 명령어를 수행하는 `branch`에서 입력된 `branch`의 `commit`을 가져온다.
- 가져온 `branch`의 `commit` 다음으로 현재 `branch`에서 작업한 `commit` 전체를 다시 생성한다.
- `merge`작업이 수행된 `commit`을 남기고 싶지 않을 때 사용한다.
- **작업 `branch`(A)에서 `rebase`를 수행하고 메인 `branch`에 `merge`한 이후를 기준으로 다른 작업자가 작업 `branch`(B)를 생성하고 작업할 때, 작업 `branch`(A)를 다시 `rebase`하면 문제가 발생함으로 기피해야한다.**

### conflict

- `rebase`도중 충돌이 발생하면

  1. 충돌을 해결하고 계속
  2. `rebase`를 중지

- 충돌을 해결하는 방법은 `merge`때와 동일하나, 충돌을 해결한 이후 `commit`을 하는게 아니라 `rebase`를 계속 진행시킨다.

  ```shell
  git rebase --continue
  ```

- `rebase` 중지

  ```shell
  git rebase --abort
  ```
