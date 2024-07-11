## hashing

### config

1. config

   - 현재 위치의 `git` 저장소의 설정이 들어있다.

2. ref/

   - 현재 `git`의 각 `commit`에 대한 해쉬값들이 저장되어 있다.
   - `branch`, `remote` 및 `tag` 정보가 저장되어 있다.

3. HEAD

   - 현재 `HEAD`에 대한 참조값이 저장되어 있다.
   - `commit` 해쉬(분리된 `HEAD`시), 현재 브런치 정보 등

4. objects/

   ```shell
   git cat-file -p <object-hash>
   ```

   - 저장소의 모든 데이터를 `해쉬`로 저장
