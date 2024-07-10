## tags

```shell
git tag
```

- 저장소의 중요한 지점을 표시하는 용도
- 릴리즈 표시용으로 사용하기도 한다.
- 특정 `commit`을 가르키는 포인터
- `tag`는 하나이상 추가가 가능하다.

### create

```shell
git tag <tag-name> [<commit-hash>]
```

- 명시된 `commit-hash`에 일반 태그 생성. `commit-hash`가 없다면 HEAD에 생성

```shell
git tag -a <tag-name> [<commit-hash>]
```

- 명시된 `commit-hash`에 주석 태그 생성. `commit-hash`가 없다면 HEAD에 생성
- 주석 태그에는 `commit`과 같이 메세지 입력이 가능하다
- `git show <tag-name>` 으로 해당 태그의 메세지를 확인할 수 있다.

### move

```shell
git tag -f <tag-name> <commit-hash>
```

- 명시된 `tag-name`을 `commit-hash` 위치로 이동시킨다.

### delete

```shell
git tag -d <tag-name>
```

- 명시된 `tag-name`을 삭제한다.

### push

```shell
git push <repository-name> <tag-name>
```

- `tag-name`을 원격 저장소에 `push`한다.

```shell
git push <repository-name> --tags
```

- 현재 저장소의 모든 `tag`들을 `push`한다.

### Semantic Versioning

- `MAJOR`: 하위 버전과의 호환성을 보장할 수 없을 때
- `MINOR`: 하위 버전과의 호환성은 유지되면서 간단한 기능이 추가될 때
- `PATCH`: 버그 및 수정사항이 반영될 때
