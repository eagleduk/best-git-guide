## undo

### checkout

```shell
git checkout <commit-hash>
```

- 분리된 `HEAD` 상태
- 특정 커밋 해시를 체크아웃
- 특정 시점의 커밋으로 이동할 수 있다.
- 이동한 시점의 상태를 확인 가능
- 이동한 시점에서 새로운 `branch` 생성이 가능하다
- 특정 `branch` 이동 `git checkout master` 또는 최근 위치에 있던 `branch`로 이동 `git checkout -` 으로 `checkout` 상태를 벗어날 수 있다.
- `commit-hash` 대신 `HEAD~<n>` 으로 현재 `HEAD` 커밋에서 `n` 번째 이전의 커밋을 선택할 수 있다.

### discard

```shell
git checkout HEAD [filename1, filename2, ... ]
```

```shell
git checkout -- [filename1, filename2, ... ]
```

- 마지막 커밋에서의 내용으로 재 설정

### restore

```shell
git restore [filename1, filename2, ... ]
```

- 명시한 파일들의 현재 변경사항을 폐기

```shell
git restore  --source <commit-hash | HEAD~n> [filename1, filename2, ... ]
```

- 명시한 파일들의 현재 변경사항을 폐기하고 선택한 커밋의 상태로 복원한다.

```shell
git restore --staged [filename, filename2, ... ]
```

- 명시한 파일들의 `staged` 추가를 제거한다.

### reset

```shell
git reset <commit-hash | HEAD~n>
```

- _soft_ `reset`
- 현재의 변경사항을 유지하면서 지정한 커밋까지의 `commit` 내역만 삭제한다.

```shell
git reset --hard <commit-hash | HEAD~n>
```

- _hard_ `reset`
- 모든 변경사항을 삭제하면서 지정한 커밋의 상태로 되돌린다.

## revert

```shell
git revert <commit-hash | HEAD~n>
```

- 명시된 커밋까지의 변경사항을 취소하고 상태를 되돌리는 새로운 커밋을 생성한다.
- 커밋을 삭제하게되면 협업에서의 문제가 발생하기 때문에 새로이 커밋을 수행한다.
- 변경사항을 되돌리게 되면 `conflict` 가 발생할 수 있다.
