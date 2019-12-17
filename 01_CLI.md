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
- `git commit`: 
- $ git config -- global user.emil
- $ git config -- global user.name
- git comit -m "first commit" : 첫번째 버전을 저장함 m 은 메세지라는 뜻. 사진찍듯이 초기 버전 저장. 
- git log : 내가 찍었던 첫번째 사진에 대한 정보가 나온다. 무엇을 저장했는지,  저장하면서남긴 메세지가 무엇인지. 
- git log --oneline : 한 줄로 보기 
- git checkout  앞 다섯글자 -> 이전 버전으로 돌아감 (현재 파일 없어짐)햣 ㅣ
- 다시 원래대로 돌려놓고 싶으면 checkout  master 를 사용함. 



사진대에 올려놓는다 git add

사진대에 올려 놓는 것을 저장한다.  git commit



- git remote add (저장소의 별명 e.g origin) (원격 저장소의 주소) -> 앞으로 이 주소에다가 올릴거야 
- git remote -v  : 정보 알기 
- git push (저장소 별명 :origin) master  : 로그인 창이 나옴 
- git remote rename `(원래 이름)``(바꿀 이름)` : 원격 저장소 이름 바꾸기