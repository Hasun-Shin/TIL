협업

(1) branch 활용

(2) fork -PR (git hub flow)

------

mkdir collabo 들어가기

git init

code -> vs code 불러오기

code . 현재폴더 기준으로 vs code 열기

README.md 파일 만들기

# 팀 소개 페이지 만들기

소개 페이지 설명서

## 1. 팀 설명

- 팀명 :
- 팀원 :

------

index.html 이라는 하나 파일 더 만들기

느낌표 탭 -> html 기본 구조 나옴

```
하다
```

git add README.md

git add index.html

다른 방법 두개 파일 한꺼번에 합치기

git add README.md index.html

또는

git add . 현재 폴더에 변경된 것 다 넣어라.

이 상태에서 commit

저장 후 push 함.

콜라보 수락 후 팀장은

collaborators 메뉴 안에 push access to the repository

branches 로 감. Branch protection rules

팀원에게 제한적인 branch 만을 줌.

팀원은 master 브랜치에 push 를 하지 못함.

깃헙에스 pull request 를 통해서 마지막에 master 와 병합함.

지금상태

first commit 하나 존재함 . 여기서부터 branch 두개 쪼개짐

하나 feature/descritption

하나 feature/home (팀원)

각자의 커밋을 찍은 다음에 git hub에 자기 branch 로 올린다.

각자의 변경분 올림.

master

feature/desc

feature/home

깃허브로 merge 하기.

내 코드를 반영. 내 코드의 차이점을 반영해주세요.

pull request 보냄.

왼쪽 상단 리뷰어에서 팀장 선택.

리뷰 리퀘스트 보내기.

팀장들은 풀리퀘스트 -> file changes 로 들어가서 답변을 달 수 있다. add ~~ 에 들어감.

코드들 확인하고 다 확인했으면 승인하기.

승인하면 맨 마지막에 request ~ 누르고 마지막으로 confirm merge 를 한다.

그 다음 delete branch 를 하면 깔끔하게 정리 된다.