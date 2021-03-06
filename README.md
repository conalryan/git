# git

```bash
echo "# git" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/conalryan/git.git
git push -u origin master
```

- .git:
  - branches:
    - (Empty Dir)
  - COMMIT_EDITMSG
  ```
  first commit
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
  c342fa2dcb1af9d058eb058f4fd783480fd8f2f4		branch 'master' of https://github.com/conalryan/git
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
  DIRC��\CÛ‰�FÂ⁄\CÛ‰�FÂ⁄��Œ™Å§�ˆ���jfb�∂◊ù+��ê��U5~≥º˘	README.mdTREE�1 0
  Í«x/mı}'�ÓZ õv�Öe_7ùYôx^Ø�ÿ¬˛Ìé–�sùÌ>S^˝
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
    0000000000000000000000000000000000000000 c342fa2dcb1af9d058eb058f4fd783480fd8f2f4 Conal RYAN <conal.ryan@amadeus.com> 1547957160 -0500	commit (initial): first commit
    ```
    - refs:
      - heads:
        - master
        ```
        0000000000000000000000000000000000000000 c342fa2dcb1af9d058eb058f4fd783480fd8f2f4 Conal RYAN <conal.ryan@amadeus.com> 1547957160 -0500	commit (initial): first commit
        ```
      - remotes
        - origin:
          - master
          ```
          0000000000000000000000000000000000000000 c342fa2dcb1af9d058eb058f4fd783480fd8f2f4 Conal RYAN <conal.ryan@amadeus.com> 1547957176 -0500	update by push
          ```
  - objects:
    - 3b:
    ```
    c5565256d5764773546c6d721b449747b14d43
    ```
    - 5d
    ```
    74de71a6bd46550678bf43cecd44d02a187d07
    ```
    - c3
    ```
    42fa2dcb1af9d058eb058f4fd783480fd8f2f4
    ```
    - info:
      - (Empty Dir)
    - pack:
      - (Empty Dir)
  - refs:
    - heads:
      - master
      ```
      c342fa2dcb1af9d058eb058f4fd783480fd8f2f4
      ```
    - remotes:
      - origin:
        - master
        ```
        c342fa2dcb1af9d058eb058f4fd783480fd8f2f4
        ```
    - tags:
      - (Empty Dir)

```bash
git log --all --graph --decorate --oneline --simplify-by-decoration
```
Prints
```bash
* c342fa2 (HEAD -> master, origin/master) first commit
```

## Append to README.md .git dir
```bash
git add .
git commit -m "second commit - Append README with .git directory after first-commit"
git push
```

- .git:
  - branches:
    - (Empty Dir)
  - COMMIT_EDITMSG
  ```
  second commit - Append README with .git directory after first-commit
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
  72132c8e6fe3029c10c8c0335b3c61059992852a		branch 'master' of https://github.com/conalryan/git
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
  DIRC      \EFT,ˇªy\EFT,ˇªy   ŒHˇ  Å§  ˆ     ^ﬂÉ∑~ª¥÷©îmXsÆsZ	˜tÕ 	README.md TREE    1 0¶˛Z/ÏÓ≈öä¶æm÷‘=‰Rgo4ì•”©OÍ}Kbﬂ∫zÿ+T0ﬁ
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
    0000000000000000000000000000000000000000 c342fa2dcb1af9d058eb058f4fd783480fd8f2f4 Conal RYAN <conal.ryan@amadeus.com> 1548041586 -0500	commit (initial): first commit
    
    c342fa2dcb1af9d058eb058f4fd783480fd8f2f4 72132c8e6fe3029c10c8c0335b3c61059992852a Conal RYAN <conal.ryan@amadeus.com> 1548044008 -0500	commit: second commit - Append README with .git directory after first-commit
    ```
    - refs:
      - heads:
        - master
        ```
        0000000000000000000000000000000000000000 c342fa2dcb1af9d058eb058f4fd783480fd8f2f4 Conal RYAN <conal.ryan@amadeus.com> 1548041586 -0500	commit (initial): first commit
        
        c342fa2dcb1af9d058eb058f4fd783480fd8f2f4 72132c8e6fe3029c10c8c0335b3c61059992852a Conal RYAN <conal.ryan@amadeus.com> 1548044008 -0500	commit: second commit - Append README with .git directory after first-commit
        ```
      - remotes
        - origin:
          - master
          ```
          0000000000000000000000000000000000000000 c342fa2dcb1af9d058eb058f4fd783480fd8f2f4 Conal RYAN <conal.ryan@amadeus.com> 1548041603 -0500	update by push
          c342fa2dcb1af9d058eb058f4fd783480fd8f2f4
        
          72132c8e6fe3029c10c8c0335b3c61059992852a Conal RYAN <conal.ryan@amadeus.com> 1548044082 -0500	update by push
          ```
  - objects:
    - 3b:
    ```
    c5565256d5764773546c6d721b449747b14d43
    ```
    - 5d:
    ```
    74de71a6bd46550678bf43cecd44d02a187d07
    ```
    - 72:
    ```
    132c8e6fe3029c10c8c0335b3c61059992852a
    ```
    - a6:
    ```
    fe5a2feceec59a8aa6be6d14d6d43de452676f
    ```
    - c3:
    ```
    42fa2dcb1af9d058eb058f4fd783480fd8f2f4
    ```
    - df:
    ```
    83b77ebbb4d6a9946d5873ae735a09f7740ecd
    ```
    - info:
      - (Empty Dir)
    - pack:
      - (Empty Dir)
  - refs:
    - heads:
      - master
      ```
      c342fa2dcb1af9d058eb058f4fd783480fd8f2f4
      ```
    - remotes:
      - origin:
        - master
        ```
        c342fa2dcb1af9d058eb058f4fd783480fd8f2f4
        ```
    - tags:
      - (Empty Dir)

## Feature A
```bash
git checkout -b feature-a
```

- .git:
  - branches:
    - (Empty Dir)
  - COMMIT_EDITMSG
  ```
  second commit - Append README with .git directory after first-commit
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
  72132c8e6fe3029c10c8c0335b3c61059992852a		branch 'master' of https://github.com/conalryan/git
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
  DIRC      \EFT,ˇªy\EFT,ˇªy   ŒHˇ  Å§  ˆ     ^ﬂÉ∑~ª¥÷©îmXsÆsZ˜tÕ 	README.md TREE    1 0¶˛Z/ÏÓ≈öä¶æm÷‘=‰Rgo4ì•”©OÍ}Kbﬂ∫zÿ+T0ﬁ
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
    0000000000000000000000000000000000000000 c342fa2dcb1af9d058eb058f4fd783480fd8f2f4 Conal RYAN <conal.ryan@amadeus.com> 1548041586 -0500	commit (initial): first commit
    c342fa2dcb1af9d058eb058f4fd783480fd8f2f4 
    
    72132c8e6fe3029c10c8c0335b3c61059992852a Conal RYAN <conal.ryan@amadeus.com> 1548044008 -0500	commit: second commit - Append README with .git directory after first-commit
    72132c8e6fe3029c10c8c0335b3c61059992852a 
    
    72132c8e6fe3029c10c8c0335b3c61059992852a Conal RYAN <conal.ryan@amadeus.com> 1548046250 -0500	checkout: moving from master to feature-a
    ```
    - refs:
      - heads:
        - feature-a:
        ```
        0000000000000000000000000000000000000000 72132c8e6fe3029c10c8c0335b3c61059992852a Conal RYAN <conal.ryan@amadeus.com> 1548046250 -0500	branch: Created from HEAD
        ```
        - master
        ```
        0000000000000000000000000000000000000000 c342fa2dcb1af9d058eb058f4fd783480fd8f2f4 Conal RYAN <conal.ryan@amadeus.com> 1548041586 -0500	commit (initial): first commit
        c342fa2dcb1af9d058eb058f4fd783480fd8f2f4
        
        72132c8e6fe3029c10c8c0335b3c61059992852a Conal RYAN <conal.ryan@amadeus.com> 1548044008 -0500	commit: second commit - Append README with .git directory after first-commit
        ```
      - remotes
        - origin:
          - master
          ```
          0000000000000000000000000000000000000000 c342fa2dcb1af9d058eb058f4fd783480fd8f2f4 Conal RYAN <conal.ryan@amadeus.com> 1548041603 -0500	update by push c342fa2dcb1af9d058eb058f4fd783480fd8f2f4 
          
          72132c8e6fe3029c10c8c0335b3c61059992852a Conal RYAN <conal.ryan@amadeus.com> 1548044082 -0500	update by push
          ```
  - objects:
    - 3b:
    ```
    c5565256d5764773546c6d721b449747b14d43
    ```
    - 5d:
    ```
    74de71a6bd46550678bf43cecd44d02a187d07
    ```
    - 72:
    ```
    132c8e6fe3029c10c8c0335b3c61059992852a
    ```
    - a6:
    ```
    fe5a2feceec59a8aa6be6d14d6d43de452676f
    ```
    - c3:
    ```
    42fa2dcb1af9d058eb058f4fd783480fd8f2f4
    ```
    - df:
    ```
    83b77ebbb4d6a9946d5873ae735a09f7740ecd
    ```
    - info:
      - (Empty Dir)
    - pack:
      - (Empty Dir)
  - refs:
    - heads:
      - feature-a
      ```
      72132c8e6fe3029c10c8c0335b3c61059992852a
      ```
      - master
      ```
      c342fa2dcb1af9d058eb058f4fd783480fd8f2f4
      ```
    - remotes:
      - origin:
        - master
        ```
        c342fa2dcb1af9d058eb058f4fd783480fd8f2f4
        ```
    - tags:
      - (Empty Dir)

```bash
git push --set-upstream origin feature-a
```

- .git:
  - branches:
    - (Empty Dir)
  - COMMIT_EDITMSG
  ```
  second commit - Append README with .git directory after first-commit
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
  [branch "feature-a"]
    remote = origin
    merge = refs/heads/feature-a
  ```
  - description
  ```
  Unnamed repository; edit this file 'description' to name the repository.
  ```
  - FETCH_HEAD
  ```
  72132c8e6fe3029c10c8c0335b3c61059992852a		branch 'feature-a' of https://github.com/conalryan/git
  72132c8e6fe3029c10c8c0335b3c61059992852a	not-for-merge	branch 'master' of https://github.com/conalryan/git
  ```
  - HEAD
  ```
  ref: refs/heads/feature-a
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
  DIRC      \EFT,ˇªy\EFT,ˇªy   ŒHˇ  Å§  ˆ     ^ﬂÉ∑~ª¥÷©îmXsÆsZ˜tÕ 	README.md TREE    1 0¶˛Z/ÏÓ≈öä¶æm÷‘=‰Rgo4ì•”©OÍ}Kbﬂ∫zÿ+T0ﬁ
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
    0000000000000000000000000000000000000000 c342fa2dcb1af9d058eb058f4fd783480fd8f2f4 Conal RYAN <conal.ryan@amadeus.com> 1548041586 -0500	commit (initial): first commit
    c342fa2dcb1af9d058eb058f4fd783480fd8f2f4 
    
    72132c8e6fe3029c10c8c0335b3c61059992852a Conal RYAN <conal.ryan@amadeus.com> 1548044008 -0500	commit: second commit - Append README with .git directory after first-commit
    72132c8e6fe3029c10c8c0335b3c61059992852a
    
    72132c8e6fe3029c10c8c0335b3c61059992852a Conal RYAN <conal.ryan@amadeus.com> 1548046250 -0500	checkout: moving from master to feature-a
    ```
    - refs:
      - heads:
        - feature-a:
        ```
        0000000000000000000000000000000000000000 72132c8e6fe3029c10c8c0335b3c61059992852a Conal RYAN <conal.ryan@amadeus.com> 1548046250 -0500	branch: Created from HEAD
        ```
        - master
        ```
        0000000000000000000000000000000000000000 c342fa2dcb1af9d058eb058f4fd783480fd8f2f4 Conal RYAN <conal.ryan@amadeus.com> 1548041586 -0500	commit (initial): first commit
        c342fa2dcb1af9d058eb058f4fd783480fd8f2f4
        
        72132c8e6fe3029c10c8c0335b3c61059992852a Conal RYAN <conal.ryan@amadeus.com> 1548044008 -0500	commit: second commit - Append README with .git directory after first-commit
        ```
      - remotes
        - origin:
          - feature-a
          ```
          0000000000000000000000000000000000000000 72132c8e6fe3029c10c8c0335b3c61059992852a Conal RYAN <conal.ryan@amadeus.com> 1548047195 -0500	update by push
          ```
          - master
          ```
          0000000000000000000000000000000000000000 c342fa2dcb1af9d058eb058f4fd783480fd8f2f4 Conal RYAN <conal.ryan@amadeus.com> 1548041603 -0500	update by push c342fa2dcb1af9d058eb058f4fd783480fd8f2f4 
          
          72132c8e6fe3029c10c8c0335b3c61059992852a Conal RYAN <conal.ryan@amadeus.com> 1548044082 -0500	update by push
          ```
  - objects:
    - 3b:
    ```
    c5565256d5764773546c6d721b449747b14d43
    ```
    - 5d:
    ```
    74de71a6bd46550678bf43cecd44d02a187d07
    ```
    - 72:
    ```
    132c8e6fe3029c10c8c0335b3c61059992852a
    ```
    - a6:
    ```
    fe5a2feceec59a8aa6be6d14d6d43de452676f
    ```
    - c3:
    ```
    42fa2dcb1af9d058eb058f4fd783480fd8f2f4
    ```
    - df:
    ```
    83b77ebbb4d6a9946d5873ae735a09f7740ecd
    ```
    - info:
      - (Empty Dir)
    - pack:
      - (Empty Dir)
  - refs:
    - heads:
      - feature-a
      ```
      72132c8e6fe3029c10c8c0335b3c61059992852a
      ```
      - master
      ```
      c342fa2dcb1af9d058eb058f4fd783480fd8f2f4
      ```
    - remotes:
      - origin:
        - master
        ```
        c342fa2dcb1af9d058eb058f4fd783480fd8f2f4
        ```
    - tags:
      - (Empty Dir)

## Add to README feature-a
```bash
git add .
git commit -m "feature-a commit-1"
git push
```
- .git:
  - branches:
    - (Empty Dir)
  - COMMIT_EDITMSG
  ```
  feature-a commit-1
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
  [branch "feature-a"]
    remote = origin
    merge = refs/heads/feature-a
  ```
  - description
  ```
  Unnamed repository; edit this file 'description' to name the repository.
  ```
  - FETCH_HEAD
  ```
  1747ef5fca36bbc54dd400965ab52df72024157a		branch 'feature-a' of https://github.com/conalryan/git 72132c8e6fe3029c10c8c0335b3c61059992852a	not-for-merge	branch 'master' of https://github.com/conalryan/git
  ```
  - HEAD
  ```
  ref: refs/heads/feature-a
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
  - index
  ```
  DIRC      \EU*pm\EU*pm   ŒHˇ  Å§  ˆ     =$jÎ?1ªÄúÜf◊'”<ÉI 	README.md TREE    1 0°V‘—~UîQ,Å·I∞a£◊Ÿ+@k''I`7]âÕÒˆÌªï<®
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
    0000000000000000000000000000000000000000 c342fa2dcb1af9d058eb058f4fd783480fd8f2f4 Conal RYAN <conal.ryan@amadeus.com> 1548041586 -0500	commit (initial): first commit c342fa2dcb1af9d058eb058f4fd783480fd8f2f4 
    
    72132c8e6fe3029c10c8c0335b3c61059992852a Conal RYAN <conal.ryan@amadeus.com> 1548044008 -0500	commit: second commit - Append README with .git directory after first-commit 72132c8e6fe3029c10c8c0335b3c61059992852a 
    
    72132c8e6fe3029c10c8c0335b3c61059992852a Conal RYAN <conal.ryan@amadeus.com> 1548046250 -0500	checkout: moving from master to feature-a 72132c8e6fe3029c10c8c0335b3c61059992852a 
    
    1747ef5fca36bbc54dd400965ab52df72024157a Conal RYAN <conal.ryan@amadeus.com> 1548097686 -0500	commit: feature-a commit-1
    ```
    - refs:
      - heads:
        - feature-a:
        ```
        0000000000000000000000000000000000000000 72132c8e6fe3029c10c8c0335b3c61059992852a Conal RYAN <conal.ryan@amadeus.com> 1548046250 -0500	branch: Created from HEAD 72132c8e6fe3029c10c8c0335b3c61059992852a 
        
        1747ef5fca36bbc54dd400965ab52df72024157a Conal RYAN <conal.ryan@amadeus.com> 1548097686 -0500	commit: feature-a commit-1
        ```
        - master
        ```
        0000000000000000000000000000000000000000 c342fa2dcb1af9d058eb058f4fd783480fd8f2f4 Conal RYAN <conal.ryan@amadeus.com> 1548041586 -0500	commit (initial): first commit c342fa2dcb1af9d058eb058f4fd783480fd8f2f4 
        
        72132c8e6fe3029c10c8c0335b3c61059992852a Conal RYAN <conal.ryan@amadeus.com> 1548044008 -0500	commit: second commit - Append README with .git directory after first-commit
        ```
      - remotes
        - origin:
          - feature-a
          ```
          0000000000000000000000000000000000000000 72132c8e6fe3029c10c8c0335b3c61059992852a Conal RYAN <conal.ryan@amadeus.com> 1548047195 -0500	update by push 72132c8e6fe3029c10c8c0335b3c61059992852a 
          
          1747ef5fca36bbc54dd400965ab52df72024157a Conal RYAN <conal.ryan@amadeus.com> 1548097695 -0500	update by push
          ```
          - master
          ```
          0000000000000000000000000000000000000000 c342fa2dcb1af9d058eb058f4fd783480fd8f2f4 Conal RYAN <conal.ryan@amadeus.com> 1548041603 -0500	update by push c342fa2dcb1af9d058eb058f4fd783480fd8f2f4
        
          72132c8e6fe3029c10c8c0335b3c61059992852a Conal RYAN <conal.ryan@amadeus.com> 1548044082 -0500	update by push
          ```
  - objects:
    - 1d:
    ```
    a15614d4d17e5594512c0c81e149b061a3d7d9
    ```
    - 3b:
    ```
    c5565256d5764773546c6d721b449747b14d43
    ```
    - 5d:
    ```
    74de71a6bd46550678bf43cecd44d02a187d07
    ```
    - 6a:
    ```
    eb3f31bb1580191f9c8666d727d33c12138349
    ```
    - 17:
    ```
    47ef5fca36bbc54dd400965ab52df72024157a
    ```
    - 72:
    ```
    132c8e6fe3029c10c8c0335b3c61059992852a
    ```
    - a6:
    ```
    fe5a2feceec59a8aa6be6d14d6d43de452676f
    ```
    - c3:
    ```
    42fa2dcb1af9d058eb058f4fd783480fd8f2f4
    ```
    - df:
    ```
    83b77ebbb4d6a9946d5873ae735a09f7740ecd
    ```
    - info:
      - (Empty Dir)
    - pack:
      - (Empty Dir)
  - refs:
    - heads:
      - feature-a
      ```
      1747ef5fca36bbc54dd400965ab52df72024157a
      ```
      - master
      ```
      c342fa2dcb1af9d058eb058f4fd783480fd8f2f4
      ```
    - remotes:
      - origin:
        - feature-a:
        ```
        1747ef5fca36bbc54dd400965ab52df72024157a
        ```
        - master
        ```
        c342fa2dcb1af9d058eb058f4fd783480fd8f2f4
        ```
    - tags:
      - (Empty Dir)

