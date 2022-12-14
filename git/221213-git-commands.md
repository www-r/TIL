# 221213

## git Process Flow and Command

working directory--git add-->staging area--git commit-->localrepo--git push-->remote repo(Github) 

## git != github

git(도구): Version Control System /
           Source Code management
github(웹서비스): Cloud Remote Repository Services 
             ex) Github, Bitbucket, Gitlab(사설 서버 구성 가능)

## Creating New Repository

1. Create new repository from github.com
2. Copy the address/url of the new repository
3. Clone the repository
   `$ git clone {repo address} `
4. Write README.md
   `$ vi README.md (open vim)
   ì (Insert mode)
   esc (back to Normal mode)
   :wq (write && quit)` 
5. Create .gitignore
6. Write .gitignore by copying from gitignore.io
7. Create other new files
8. Add and commit frequently
  `$ git add {repo name}
   $ git commit {repo name}`
9. Push commits to Github 
   (origin is just a name for URL)
   `$ git push origin main`
10. Check Github if everything is upadated
 
## Coventional Commits (when naming the title of the commit)

- commit 의 제목은 commit 을 설명하는 하나의 구나 절로 완성  
- Importance of Capitalize
- Add Prefix at titles
  - feat : 기능 개발 관련
  - fix : 오류 개선 혹은 버그 패치
  - docs : 문서화 작업
  - test : test 관련
  - conf : 환경설정 관련
  - build : 빌드 관련
  - ci : Continuous Integration 관련
  - BREAKING CHANGE : 되돌이킬 수 없는 변화를 주었을 때
- 좋은 예시 : Github Angular 

### commit 할 때 기억해야 할 것

- commit 은 동작 가능한 최소단위로 자주 할 것
- 해당 작업단위에 수행된 모든 파일 변화가 해당 commit 에 포함되어야 함
- 모두가 이해할 수 있는 log 를 작성할 것
- 제목은 축약하여 쓰되(50자 이내), 내용은 문장형으로 작성하여 추가 설명을 할 것( 이 commit 의 구성과 의도를 충실히 작성)
- 제목과 내용은 한 줄 띄워 분리할 것


