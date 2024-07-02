## merge

### fast-forward

- 빨리 감기 병합, 따라잡기 병합
- 가져오고자 하는 `branch` 에서 수행
- 가져오고자 하는 `branch`에 커밋이 없고 가져올 `branch`에 커밋이 있을 때
- 가져올 `branch`의 커밋을 가져오고자 하는 `branch`에 가져오는 것

```shell
git merge <branch-name>
```

### merge

- 병합 커밋
- 합치고자 하는 `branch` 에서 수행
- 가져오고자 하는 `branch`에 커밋이 있고 가져올 `branch`에 커밋이 있을 때
- 가져오고자 하는 `branch`와 가져올 `branch`의 수정 사항에 대하여 서로 중복되지 않을 때
- `Git`에서 자동으로 두 `branch`의 수정사항을 적용한다.
- 병합 커밋의 부모 커밋은 2개를 가진다.

```shell
git merge <branch-name>
```
