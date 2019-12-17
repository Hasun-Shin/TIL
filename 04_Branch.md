# Branch

원래 하나의 가지 즉, master 에서 작업을 해오고 있었다.

`git branch` : 지금 연결된 세계=branch 를 보여줌. -> 주로  (master)라고 뜬다.  

`git branch new` : 새로운 'new' 라는 이름의 branch  형성

-> 형성 후에 git branch 하면 새로운 new 브랜치가 형성된 것을 알 수 있다. 총, master, new 이렇게 형성됨 

`git switch new` : master 에서 new 라는 branch로 옮겨진다. 

즉, 코드 끝 단의 하늘색의 괄호 안에는 내가 지금 속한 세계, 작업하고 있는 환경 <=> branch를 보여주고 있다. 

`head` :일종의 포인터 역할.  만약, 지금 master branch 에 있으면 head 는 master 를 향하게 된다.

--------

## 예시 작업

- master branch  에서 a.txt, b.txt, c.txt 만든다.
- git branch new 를 만들어준다.
- new branch 에서 d.txt 를 만들어준다. 총 new 에는 a,b,c,d 텍스트 파일이 생겨진다.
- new 에서 만든 새로운 파일 d.txt 는 master 에서는 보여지지 않는다.  a,b,c 만 있음.
- master로 switch 하여 master 에서 e.txt 를 만들었다.  총 **master** 에는 **a,b,c,e** 만 있다.

- 다시 new로 switch 한다. **new** 에는 최종적으로 **a,b,c,d** 만 있다.

----

## 내가 어느 branch 에 속한지 아는 방법

1. 끝 단 branch 이름 (e.g (master))
2. git log 에서 head가 가리키는 것
3. git branch 에서 별표가 있는 것



## Merge

### 이제 두  branch인 new와 master  를 합치려면?

- 먼저 내가 master 에서 있는 입장에서 !!!!!!! new 와 병합한다. 
  - git switch master 의 상태로 옴
  - `git merge new`  실행 

만약에 , local 화면으로 (돌이킬 수 없는 강으로..) 가게 된다면 

`esc 연타` + `콜론:` + `wq`로 나가기 !!!!

------------

## merge 시나리오

### 1. Fast Forward Merge

- 브랜치 분기가 일어났지만, merge 시점에서 branch 한 쪽에서만 commit들이 쌓여져 있는 경우
  - (ex, new에만 commit이 있고, master에는 없었을 때 )
- 같은 파일 명 조금만 다른 내용인데도 merge 가능
  - fast forward merge 의 조건 : master 에서 commit이 하나도 생기지 않을 때.  분기 이후 새로운 branch 에서만의 작업이 이뤄졌을 때 

- `git merge new --no--ff` : fast foward 없이 그냥 merge 하기. 





### 2. Auto-merge

- merge 시점에 양쪽 branch에 commit들이 쌓여 있지만, conflict 가 발생하지 않는 경우



### 3. Merge conflict 발생

merge 시점에 양쪽 branch에 commit들이 쌓여 있고, conflict 가 발생하는 경우 

- 동일 파일 내에(파일명이 같음) 상충하는 내용이 있을 경우 

그러므로, 여러 사람들과 동일 작업을 할 때 

같은 파일을 건들지 말아야 한다. 

협업시 한 사람의 작업이 끝난 후에 해야 한다. 



---------

**TIP!!**

`git branch -d` (지울 branch 이름) : 브랜치 삭제 

`$ git switch -c neo` : neo branch 를 생성하면서 바로 그 곳에 속하기. switch neo 할 필요가 없다.  

-------------



github repository 로 push 하기.

master branch 만 있다면

test branch 도 push 시킴



