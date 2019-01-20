# GIT

```bash
git init
```

- .git:
  - branches:
    - (Empty Dir)
  - config
    ```
    [core]
      repositoryformatversion = 0
      filemode = true
      bare = false
      logallrefupdates = true
      ignorecase = true
      precomposeunicode = true
    ```
  - description
    ```
    Unnamed repository; edit this file 'description' to name the repository.
    ```
  - HEAD
    ```
    ref: refs/heads/master
    ```
  - hooks:
    - update.sample
    - prepare-commit-msg.sample
    - pre-receive.sample
    - pre-rebase.sample
    - pre-push.sample
    - pre-commit.sample
    - pre-applypatch.sample
    - post-update.sample
    - commit-msg.sample
    - applypatch-msg.sample
  - info:
    - exclude
    ```
    # git ls-files --others --exclude-from=.git/info/exclude
    # Lines that start with '#' are comments.
    # For a project mostly in C, the following would be a good set of
    # exclude patterns (uncomment them if you want to use them):
    # *.[oa]
    # *~
    .DS_Store
    ```
  - objects:
    - info:
      - (Empty Dir)
    - pack:
      - (Empty Dir)
  - refs:
    - tags:
      - (Empty Dir)
    - heads:
      - (Empty Dir)

## Add README.md (the stuff above)
```bash
git remote add origin https://github.com/conalryan/git.git
git add .
git commit -m "Init"
git push --set-upstream origin master
```
- .git:
  - branches:
    - (Empty Dir)
  - COMMIT_EDITMSG
  ```
  README
  ```
  - config
    ```
    [core]
      repositoryformatversion = 0
      filemode = true
      bare = false
      logallrefupdates = true
      ignorecase = true
      precomposeunicode = true
    [remote "origin"]
	    url = https://github.com/conalryan/git.git
	    fetch = +refs/heads/*:refs/remotes/origin/*
    [branch "master"]
	    remote = origin
	    merge = refs/heads/master
    ```
  - description
    ```
    Unnamed repository; edit this file 'description' to name the repository.
    ```
  - FETCH_HEAD
  ```
  ce14b25fef71390adeecbec6487dcad3b8357a35		branch 'master' of https://github.com/conalryan/git
  ```
  - HEAD
    ```
    ref: refs/heads/master
    ```
  - hooks:
    - update.sample
    - prepare-commit-msg.sample
    - pre-receive.sample
    - pre-rebase.sample
    - pre-push.sample
    - pre-commit.sample
    - pre-applypatch.sample
    - post-update.sample
    - commit-msg.sample
    - applypatch-msg.sample
  index
  ```
  DIRC      \CÍ∞&]œ˝\CÍ∞&]œ˝   Œ™  Å§  ˆ     è5I°Áéæ˙gqtå*l_ Œ‰n 	README.md TREE    1 0
  N◊P4¢“EØÇ√9˚≥HAüf$9bà»Z,\êçBò§JΩË§Ëﬁ
  ```
  - info:
    - exclude
    ```
    # git ls-files --others --exclude-from=.git/info/exclude
    # Lines that start with '#' are comments.
    # For a project mostly in C, the following would be a good set of
    # exclude patterns (uncomment them if you want to use them):
    # *.[oa]
    # *~
    ```
  - logs:
    - HEAD
    ```
    0000000000000000000000000000000000000000 915cd1b852e32f3874fcfe9112a8a06171bf9b89 Conal RYAN <conal.ryan@amadeus.com> 1547954760 -0500	commit (initial): README
    915cd1b852e32f3874fcfe9112a8a06171bf9b89 ce14b25fef71390adeecbec6487dcad3b8357a35 Conal RYAN <conal.ryan@amadeus.com> 1547954873 -0500	commit: README
    ```
    - refs:
      - heads:
        - master
        ```
        0000000000000000000000000000000000000000 915cd1b852e32f3874fcfe9112a8a06171bf9b89 Conal RYAN <conal.ryan@amadeus.com> 1547954760 -0500	commit (initial): README
        915cd1b852e32f3874fcfe9112a8a06171bf9b89 ce14b25fef71390adeecbec6487dcad3b8357a35 Conal RYAN <conal.ryan@amadeus.com> 1547954873 -0500	commit: README
        ```
      - remotes
        - origin:
          - master
          ```
          0000000000000000000000000000000000000000 915cd1b852e32f3874fcfe9112a8a06171bf9b89 Conal RYAN <conal.ryan@amadeus.com> 1547954774 -0500	update by push
          915cd1b852e32f3874fcfe9112a8a06171bf9b89 ce14b25fef71390adeecbec6487dcad3b8357a35 Conal RYAN <conal.ryan@amadeus.com> 1547954881 -0500	update by push
          ```
  - objects:
    - info:
      - (Empty Dir)
    - pack:
      - (Empty Dir)
  - refs:
    - heads:
      - master
      ```
      ce14b25fef71390adeecbec6487dcad3b8357a35
      ```
    - remotes:
      - origin:
        - master
        ```
        ce14b25fef71390adeecbec6487dcad3b8357a35
        ```
    - tags:
      - (Empty Dir)
