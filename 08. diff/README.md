## diff

```shell
git diff
```

- 깃에서의 변경 사항들을 보여주는 명령어
- 마지막 커밋 이후 `stage`에 추가되지 않은 변경사항을 보여준다.

### HEAD

```shell
git diff HEAD
```

- 마지막 커밋 이후 워킹디렉토리의 모든 변경사항을 보여준다.
- `stage`에 추가되어 있더라도 변경사항을 보여준다.

### stage

```shell
git diff --staged
```

```shell
git diff --cached
```

- `stage`에 등록된 변경사항만 보여준다.

### file

```shell
git diff [filename1 filename2 ...]
```

```shell
git diff HEAD [filename1 filename2 ...]
```

```shell
git diff --stage [filename1 filename2 ...]
```

- 명시한 `file`에 대한 변경사항을 보여준다.

### branch

```shell
git diff branch1..branch2
```

```shell
git diff branch1 branch2
```

- 명시한 `branch` 간에 변경사항을 보여준다.
- 명시 순서에 따라 변경사항 내용이 달라진다.

### commit

```shell
git diff commit1..commit2
```

```shell
git diff commit1 commit2
```

- 명시한 `commit` 간에 변경사항을 보여준다.
- 명시 순서에 따라 변경사항 내용이 달라진다.
- `commit` 의 _hash_ 값으로 비교 한다.

### [Exercise](https://plum-poppy-0ea.notion.site/Git-Diff-Exercise-f7829bd2783940cea14239022a6c37a9)
