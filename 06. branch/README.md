## branch

- `branch`에 등록된 파일 중 수정사항이 `stage` 나 `commit` 이 되어 있지 않으면, `branch` 이동이 불가능하다.
- `branch`에 등록되지 않은 파일은 `branch`이동 시에도 유지된다.

```shell
git branch
```

### HEAD

- 가장 마지막에 커밋한 것
- 현재 위치를 가리키는 포인터
- 브랜치 레퍼런스

### create

```shell
git branch <branch-name>
```

### switch

```shell
git switch <branch-name>
```

### checkout

- `branch` 이동의 다른 방법

```shell
git chechout <branch-name>
```

### create & switch

```shell
git switch -c <branch-name>
```

```shell
git checkout -b <branch-name>
```

### delete

- 삭제할 대상이 아닌 `branch` 에서 수행

1. `branch` 병합이 완료 되었을 때

   ```shell
   git branch -d <branch-name>
   ```

2. `branch` 강제 삭제
   ```shell
   git branch -D <branch-name>
   ```

### rename

- 변경할 `branch` 에서 수행

```shell
git branch -m <branch-name>
```
