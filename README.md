# 개인정보보호법 키워드에 관한 여론 분석

## 사용 언어 및 기술 스택:

언어 : python / 분석 환경 : Jupyter notebook
언어 패키지 : 한국 konlpy, 영어 nltk, 중국 jieba
분석 방법론 : TF-IDF / LDA
주요 사용 패키지 : 
- 크롤링 - selenium, BeautifulSoup, requests 등
- 분석 - pandas, numpy, gensim, spacy, re, sklearn, en_core_web_sm 등

## 분석 매체 및 키워드:

### 한국 개인정보보호법
- 매체: 조선일보, SBS, 트위터
- 키워드: 개인정보보호법

### 유럽 GDPR
- 매체: EuroNews, DWnews, 트위터
- 키워드: GDPR

### 중국 个人信息保护法
- 매체: 인민일보, CCTV, 웨이보
- 키워드: 个人信息保护法

## 분석 결과:

### 한국
- 시간별 분포도:
  - ![image](https://user-images.githubusercontent.com/58875794/182599832-0604114e-6f09-4ec8-9117-5e2d823545a8.png)
  - 위에서 아래로 조선일보, SBS, 트위터 순으로 나열
  
- TF-IDF 워드클라우드:
  - 조선일보 워드클라우드
  - ![image](https://user-images.githubusercontent.com/58875794/182599896-21c3c7e5-d441-4317-8b0b-b00c4017ccad.png)
  - SBS 워드클라우드
  - ![image](https://user-images.githubusercontent.com/58875794/182599922-d4e6f1dd-feac-4512-87b0-b22562f78435.png)
  - 트위터 워드클라우드
  - ![image](https://user-images.githubusercontent.com/58875794/182599952-69377024-2a9f-4a6e-8754-c158fb197e00.png)

- LDA 토픽 모델링
  - 조선일보 토픽별 분포도 
  - ![image](https://user-images.githubusercontent.com/58875794/182599995-ad0fc300-fc97-4a34-9fdf-bc50c0c9d66e.png)
  
  - SBS 토픽별 분포도
  - ![image](https://user-images.githubusercontent.com/58875794/182600032-29d7d389-8875-44eb-aa93-81b761131d10.png)
  
  - 트위터 토픽별 분포도
  - ![image](https://user-images.githubusercontent.com/58875794/182600052-ea8a7e31-1ef4-4756-a4e7-5838ea4dbc6c.png)

### EU
- 시간별 분포도:
  - ![image](https://user-images.githubusercontent.com/58875794/182600257-320b9daa-7ecf-474d-8a02-f9751e6abb8e.png)
  - 위에서 아래로 DW news, Euronews, 트위터 순으로 나열
  
- TF-IDF 워드클라우드:
  - DWnews 워드클라우드
  - ![image](https://user-images.githubusercontent.com/58875794/182600125-ee402d61-6518-416c-b5cb-f0b5134a00f6.png)
  - Euronews 워드클라우드
  - ![image](https://user-images.githubusercontent.com/58875794/182600148-3d7a7510-ba96-4983-b60a-e1bed9460f63.png)
  - 트위터 워드클라우드
  - ![image](https://user-images.githubusercontent.com/58875794/182600162-ee24ab59-b2bc-42a8-aa78-8a6022addc86.png)

- LDA 토픽 모델링
  - DW news 토픽별 분포도 
  - ![image](https://user-images.githubusercontent.com/58875794/182600279-d2e8e1c9-10be-4202-b43d-c05ee9ea23c4.png)
  
  - Euronews 토픽별 분포도
  - ![image](https://user-images.githubusercontent.com/58875794/182600298-3d0aa24e-d932-4f3c-89ec-9edf084db335.png)
  
  - 트위터 토픽별 분포도
  - ![image](https://user-images.githubusercontent.com/58875794/182600324-59d6c20d-d297-4abd-a722-0ca90ffa8c17.png)


### 중국
- 시간별 분포도:
  - ![image](https://user-images.githubusercontent.com/58875794/182598942-8af69c11-2291-412b-ad99-7419f18283f6.png)
  - 위에서 아래로 인민일보, CCTV, 웨이보 순으로 나열
  
- TF-IDF 워드클라우드:
  - 인민일보 워드클라우드
  - ![image](https://user-images.githubusercontent.com/58875794/182599493-56f2578a-e59c-46e7-88ae-660a2e75d735.png)
  - CCTV 워드클라우드
  - ![image](https://user-images.githubusercontent.com/58875794/182599528-41d6669e-2a7e-4c4d-aa01-1d5226c78b12.png)
  - 웨이보 워드클라우드
  - ![image](https://user-images.githubusercontent.com/58875794/182599550-1d126571-54f7-42ab-93b9-aa492f545468.png)

- LDA 토픽 모델링
  - 인민일보 토픽별 분포도 
  - ![image](https://user-images.githubusercontent.com/58875794/182599661-31e7c2b0-275b-49d4-96c0-1093f9cbe52b.png)
  
  - CCTV 토픽별 분포도
  - ![image](https://user-images.githubusercontent.com/58875794/182599748-cc16a00b-92df-4909-8821-17d20983257b.png)
  
  - 웨이보 토픽별 분포도
  - ![image](https://user-images.githubusercontent.com/58875794/182599777-5193ecce-d7a5-4922-a3bf-b930d210ef6e.png)


### 전체 결과:
- 첫번째, 중국과 유럽 매체의 여론 집중도는 해당 정책의 시행 여부 및 시행 시점에 크게 영향을 받는 반면에 한국 매체는 사회적 이슈 발생 여부에 크게 영향을 받았습니다.
- 두번째, 모든 지역의 매체가 정책 관련 사회적 이슈에 관심이 많았습니다.
- 세번째, 뉴스 매체의 목적은 정확한 정보전달, SNS는 비교적 주관적인 의견이 많고 의견을 나누는 성향이 강했습니다.
