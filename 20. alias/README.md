## alias

```text
[alias]
    s = status
    l = log
```

```shell
git config --[global|local] alias.<shotchutname> <git-command>
```

- `home` 위치에 있는 `.gitconfig`파일을 수정하여 여러 설정을 수정할 수 있다.
- 해당 저장소에만 추가하고 싶은 경우에는 저장소 내의 `.git`폴더 안에있는 `config` 파일을 수정하여 설정을 적용시길 수 있다.
- 인자가 있는 명령어의 경우에는 자동으로 연결한 명령어 뒤에 붙여진다.

  ```shell
     git config --global alias.a add
     git a file1 file2 = git add file1 file2
  ```

### alias references

1. [Git Alias](https://github.com/GitAlias/gitalias)
2. [The Ultimate Git Alias Setup](https://gist.github.com/mwhite/6887990)
3. [durdn-nicola paolucci](https://www.durdn.com/blog/2012/11/22/must-have-git-aliases-advanced-examples/)
