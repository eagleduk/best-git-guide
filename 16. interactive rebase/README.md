## interactive rebase

```shell
git rebase -i HEAD~n
```

- 이력 재구성
- `commit` 메세지 편집
- `commit` 내용 변경
- `commit` 변경
- `commit` 순서 재구성
- 작업한 `branch`를 공유하기 전 이력을 다듬고 정리할때 사용
- 최신 `commit`(HEAD)에서 갯수 선택으로 조절
- 명령어 수행시 선택한 `commit`의 작업을 선택할 수 있다.

1. pick
2. reword
   - `commit` 메세지 재 설정
3. edit
4. fixup
   - 선택 `commit`의 코드를 이전 커밋으로 병합하고 메세지만 제거
5. drop
   - 선택 `commit`을 제거 코드도 이전 `commit` 상태로 되돌린다.
