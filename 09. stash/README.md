## stash

```shell
git stash
```

- 커밋하지 않은 변경사항들을 임시 저장하는 것.
- 불필요한 커밋으로부터 이력을 관리할 수 있다.
- 커밋하지 않은 모든 변경사항, 등록했거나 등록하지 않는 변경사항을 모두 임시 저장
- `stash`에 등록된 변경사항은 보이지는 않지만 추후에 `stash`에 등록된 변경사항을 되찾아올 수 있다.

### pop

```shell
git stash pop
```

- 가장 최근에 `stash`에 저장한 변경사항들을 삭제하고 어디에 있던지(`branch`) 복사본에 다시 적용

### apply

```shell
git stash apply
```

- 가장 최근에 `stash`에 저장한 변경사항들을 적용하고 삭제는 하지 않는다.
- 여러 `branch`에 적용할 수 있다.

### conflict

- `stash`를 적용할 때에도 충돌이 일어날 수 있다.
- 해결 방법은 `merge`와 동일

### list

```shell
git stash list
```

- 저장된 `stash` 목록을 확인한다.

  > stash@{0}: ~
  >
  > stash@{1}: ~
  >
  > stash@{2}: ~

- `pop` 및 `apply` 시 적용한 `stash` ID를 입력하면 해당하는 `stash` 항목을 가져온다.

### drop

```shell
git stash drop <stash@{}>
```

- 입력한 `stash`의 항목을 제거한다.

### [Exercise](https://plum-poppy-0ea.notion.site/Stashing-Exercise-b6b4ac460c0a4798845de177fc1eb86d)
