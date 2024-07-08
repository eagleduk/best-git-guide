## remote

```shell
git branch -r
```

- 원격 저장소가 연결 중일 때 원격 저장소의 모든 `branch` 정보를 확인한다.

```shell
git switch <remote-branch-name>
```

```shell
git checkout --track <remote-name/remote-branch-name>
```

- 원격 저장소의 `branch` 가 존재하면 `branch`의 최신 정보를 가져온다.

## fetch

```shell
git fetch <remote-name> [<remote-branch-name>]
```

- 원격 저장소에 있는 **최신 정보**만을 로컬 저장소에 다운로드한다.
- `checkout <remote-name/remote-branch-name>` 명령으로 다운로드한 `remote-branch(<remote-name/remote-branch-name>)`의 수정사항 등을 확인할 수 있다.

## pull

```shell
git pull [<remote-name> <remote-branch-name>]
```

- 원격 저장소의 내용을 로컬 저장소로 다운받아 적용한다.
- `fetch + merge`
- **어떤 브랜치에 있던 현재 `pulling down` 하는 곳으로 변경사항이 병합된다.**
- 목적지를 입력하지 않으면 자동으로 `remote-name` 과 현재 `branch`를 자동으로 설정한다.

### conflict

- 원격 저장소의 수정사항과 로컬 저장소의 수정사항이 겹치면 발생한다.
- `pull` 명령으로 원격 저장소의 수정사항을 다운받고 `merge` 작업 이후에 `commit`, `push` 순으로 작업하여 원격 저장소를 업데이트 해준다.
