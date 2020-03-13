# CLI

커멘드 라인 인터페이스



## 터미널 명령어들

- `ls`:  폴더 내부의 파일 & 폴더를 나열
- `pwd`: 현재 폴더 경로 출력

- `mkdir[폴더명]`: 폴더 생성

```shell
$ mkdir TIL
```

- `cd`[폴더명]: (Change Directory)  폴더 변경 

```shell
$ cd TIL/
```

- `cd ..` : 상위 폴더로 이동 
- `git init` : 해당 현재 폴더에서 git 을 시작한다. 
- `git status`:  git 의 현재상태를 묻는다.
- `touch[파일명]`: 파일을 새로 생성함. 
- `rm[파일명.확장자]` : 파일 삭제 
- `git add[파일명]`: 사진대에 올려놓음.  
- `git commit`: 사진대에 올려 놓는 것을 저장한다.
- `git`설정 (user,name & user.email) : 최초 1회 설정

``` shell
- `$ git config -- global user.emil`"Hasun Shin"
- `$ git config -- global user.name `"hahahasony@naver.com"
```

- `git comit -m` "first commit" : 첫번째 버전을 저장함 m 은 메세지라는 뜻.

  즉, "first commit" 이라는 멘트를 달아 초기 버전 저장. 

- `git log` : 내가 찍었던 첫번째 사진에 대한 정보가 나온다. 무엇을 저장했는지,  저장하면서남긴 메세지가 무엇인지. 

- `git log --oneline` :  log 정보를 한 줄로 출력해서 보기  
- git reset --mixed HEAD^ : commit을 취소하고 해당 파일들은 unstaged 상태로 워킹 디렉터리에 보존
-  git reset HEAD^ : 위와 동일
-  git reset HEAD~2 // 마지막 2개의 commit을 취소




- `git checkout`(git log에서 출력된 코드에서)  앞 다섯글자  : 앞 다섯글자에 해당하나는 이전 버전으로 돌아감 (현재 파일 없어짐)

- `checkout  master` : `git checkout` 을 하기 전 다시 원래대로 돌려놓고 싶으면 사용함.

- `git remote add` (저장소의 별명 e.g origin) (원격 저장소의 주소) : 앞으로 이 주소에다가 올릴것이라고 선언함. 

- `git remote -v`  :  저장소 장소가 어딘지 정보 알기 

- `git push (저장소 별명 :origin) master` 
  
  - 처음에 업로드 할 때는 로그인 창이 나오지만, 그 후에는 저장소에 자연스럽게 업로드가 된다. 
  
- `git remote rename `(원래 이름)(바꿀 이름)` : 원격 저장소 이름 바꾸기

- `rm -r .git` : git 파일을 삭제함. 

- `mv`  이동할파일/이동할 폴더 

- `ls -a` : 숨겨진 git 폴더 까지 다 볼 수 있다. 

- `git branch` : 현재 어떤 branch 에 연결되어 있는지 보여준다. 

- `git branch -d` (지울 branch 이름) : 브랜치 삭제

- `$ git switch -c neo`

-  `git remote add origin https://github.com/Hasun-Shin/conflict.git(주소)` :원격저장소 생성 

- `rm -rf ./.git` : git생성한 것을 삭제함

- `esc 세번, :wq` : 돌이킬 수 없는 강을 건널 때 빠져나옴 


