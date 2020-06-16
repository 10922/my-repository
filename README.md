
# 가짜 뉴스 판별 _ 팀 해피
- 문이현([@10922](https://github.com/10922))
- 윤주석([@YUNJUSEOK](https://github.com/YUNJUSEOK))
- 김민철([@201810759](https://github.com/201810759))
- 이우형([@dngud9701](https://github.com/dngud9701))
 
---

### Ⅰ. 주제와 필요성
   __1. 주제__
- 가짜 뉴스 판별
- 정치적인 목적이나 경제적인 이득을 위해 의도적으로 언론 보도의 형식을 하고 유포하는 거짓 정보
- 일반적인 뉴스와 달리, 가짜 뉴스는 주관적이고 편향적이기 때문에 수집한 데이터셋을 바탕으로 학습한다면 판별하는 일이 가능하다고 예측

---

### 2. 필요성

- 정보를 인터넷으로 접하는 현대 사회에서 비판적이고 능동적으로 뉴스를 받아들일 수 있도록, 기사를 분석하고 검증하는 절차를 통해 __올바른 뉴스를 제공__
- 쟁점이 되는 사안에 관해 가짜 뉴스를 생산하고 유포하거나 여론을 조작하고 선동하는 현상에 대처하면서, __언론 보도의 공정성을 확보하고 신뢰성을 향상__

---

### 3. 기술 개발 전략

- 진위 판별을 거쳐 레이블화된 영문 데이터셋을 활용
- 입력과 출력이 하나의 시퀀스이므로 이 처리를 위해 고안된 RNN 계열 모델을 사용
- 주어진 문장을 토큰화 · 정제 · 정규화 방안을 이용하여 데이터 전처리
- Bag of Words 방법으로 각각의 빈도를 파악하고 단어에 맞는 수치를 입력
- 각각의 문장을 최대 길이에 맞춰 패딩

---

### 4. 사업화 전략

- 웹사이트를 통해 서비스를 제공
- 더욱 심화적인 기능은 부분적으로 유료화

---

### 5. 역할

- 기획

  - 주제를 선정하고 필요성을 분석
  - 조사하고 수집한 자료를 바탕으로 서비스를 설계
  - 개발을 위해 필요한 기술을 연구

- 개발 
  - 상용화된 FAKE-NEWS 데이터셋을 활용
  - 토큰화 · 정제 · 정규화 방안을 이용하여 데이터 전처리
  - LSTM을 기반으로 y^산출을 통해 가짜 뉴스를 판별
 

- 서비스 
   - 웹사이트를 개설하고 사용자에게 서비스를 제공

---

### 6. 일정 계획

- 주제 선정
- 가짜 뉴스 판별을 위한 자료 조사
- 알고리즘에 필요한 Feature 조사
  - 문장의 언어적 특성, 출처 및 분야별 키워드
- 데이터셋에 관한 자료 조사
- 전처리에 관한 자료 조사
  - 기본 전처리 구조, TF-DF 및 WORD2VEC
- 전처리를 위한 토론
- 기술 개발 전략 구체화
- 트레이닝
- 테스트 및 개선
- 서비스 구현

---

