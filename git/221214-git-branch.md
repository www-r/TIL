# 221214 Git Branch

## git commands

- git branch  
    :show available local branch
- git branch -r
    :show available remote branch
- git branch -a
    :show available All branch
- git branch {new branch name}
    :create new branch
- git switch {branch name} 
    :switch to {branch name} 
- git merge {changed branch} (pull from the main)
    : merge {changed branch} with the original one
- git branch -D {branch name}
    : delete {branch name}
- git push origin {branch name}
    : push {branch name} to origin(address) 

- git push -u origin develop
    : (when it is first time pushing to the branch-de      velop) push to branch develop
- git flow feature start
 ,git flow feature end
    :(when making changes) mostly used

## merge conflicts

내용이 달라서 그런것이니, 수정하면 된다. 
 
## branching models

1. git flow
  :(hotfix)-main-(release)-develop-feature
     - hotfix: merge right into branch main(not common)
  - mostly used
  - precise to divide/sort branchs
2. github flow
3. gitlab flow

## Rename &&  Revert && Reset

1.

- Revert : 이전 상태로 되돌리는 것 -> 흔적이 남는다
- Reset : (not recommended) 존재 자체를(있었다는 사실조차) 지우는 것

2. commands

- git switch -- ,
  git switch -- {file name}
    : undo
- git reset HEAD {file name}
    : unstage latest work of {file name}
- git restore {file name}
    : unstage {file name} (only added ones, not commited)
- git rm -f {file name}
    : unstage and remove {file name} 
- git revert --no-commit HEAD~3..
    : 현재 HEAD에서 직전의 commit 3개를revert 
- git commit --amend
   : edit latest commit
