## 예측 모델링

- suprervised segmentation (감독 세분화 ) : target value 를 가지고 있음. 
- 이를 수행하기 위해서는 속성들(attribute 혹은 feature vector)이 target value에 끼치는 영향들을 알아봐야 한다. 



###  모델

- 어떤 목적 달성을 위해 실 세계를 단순하게 표현한 것. 

  예 : 

  - 네비게이션 . 어느 길을 지날 때 가로수 나무 개수 나오지 않음. 건물모양도 랜드마크 아니고서는 생략함. 즉, 목적에 안 맞는 것은 삭제함.  

  - 만약에 국영수 윤리 에서 윤리가 영향력 작으면 삭제할 수 있음. 알고리즘의 속도가 빨라짐. 삭제할 수 있다는 근거를 어디서 찾을 수 있을까? -> **feature selection** 

- 모델유도 Model induction
  - 데이터로부터
  - 귀납법
  - 범용규칙
  - 유도알고리즘, 학습자
  - -> 즉, 데이터들을 하나씩 보면서 판단. 



## Supervised Segmenataion

- 엔트로피 Entropy

  - 어떤 집합에 대한 무질서 정도를 측정 

  - 분류 예측에서는 엔트로피가 0 일때 완전히 잘 분류했다고 볼 수 있다. 

    

- 정보 증가량 Information Gain



- 의사결정 나무 decision tree

