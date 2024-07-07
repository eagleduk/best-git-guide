## Github

### clone

```shell
git clone <git-repository-url>
```

### [ssh](https://docs.github.com/en/authentication/connecting-to-github-with-ssh)

### remote

1. Git Repository Url 확인

```shell
git remove -v
```

2. Git Repository Url 연결

```shell
git remote add <remote-name> <git-repository-url>
```

- `git-repositoy-url`을 `name`으로 기억

### push

```shell
git push <remote-name> <branch>
```

```shell
git push <remote-name> <local-branch>:<git-repository-branch>
```

- `local-branch` 의 커밋을 `git-repository-branch` 에 업로드

```shell
git push -u <remote-name> <branch | local-branch:git-repository-branch>
```

- `git` upstream 설정
- 최소 `-u` 옵션을 사용하여 `push` 시 `remote-name` 과 `branch` 정보는 저장하여 `git push` 단축어를 사용할 수 있게 한다.
