## reflog

```shell
git reflog show|expire|delete|exists
```

- `git`은 모든 행위에 대하여 `logs/`에 기록한다.
- 단 저장소의 모든 행위가 아닌 **local** 저장소에 한하여 기록한다.
- 모든 `log`는 만료기한이 존재한다.
- `reset --hard`로 지워버린 `commit`과 변경사항도 `reflog`에는 기록되어 있기 때문에, `reset` 또는 `checkout`으로 그 시점의 상태로 회귀하거나 상태확인이 가능하다.
- `rebase -i`로 지워버린 `commit`과 변경사항도 `reflog`에는 기록되어 있기 때문에, `reset` 또는 `checkout`으로 그 시점의 상태로 회귀하거나 상태확인이 가능하다.
- `reflog`로 지워버린 변경사항을 되돌린 이후에도, 다시 지워버린 변경사항으로 회귀할 수 있다.
