# Topic_Modeling

- 한두개의 문서가 아닌 수천개의 경향성 파악용
- Topic model: 문서집합의 추상적인 '주제'를 발견하기 위한 통계적 모델 중 하나로 </br>
text 본문의 **숨겨진 의미구조**를 발견하기 위해 사용되는 text mining 기법 중 하나
- 문헌 내 어떤 주제가 들어있고, 주제 간의 비중이 어떤지는 문헌 집합 내의 단어 통계를 수학적으로 분석함으로써 알아낼 수 있기에 확률적 토픽모델이라고도 불림
- 여러 Topic model algorithm중 LDA 위주로 

## LDA(Latent Dirichlet Allocation, 잠재 디리클레 할당)
- 주어진 문서에 어떤 주제들이 존재하는지 서술하는 확률적 토픽모델 기법 중 하나
- 미리 알고 있는 주제별 단어 수 분포를 바탕으로 주어진 문서에서 발견된 단어 수 분포를 분석해 어떤 주제들을 다루고 있을지를 예측하는 모델
- workflow </br>
  1. data 이해
  2. text 전처리
  3. TF-IDF 행렬 만들기
  4. LDA학습 및 결과분석
  
### Text preprocessing
- text를 자연어 처리를 위해 용도에 맞도록 표준화하는 작업
- text내 정보는 유지하고 중복을 제거해 분석 효율성을 높이기위함
- tokenization, 품사 tagging, 개체명 인식, 원형복원, 불용어 처리 등

### TF-IDF 행렬 만들기 (Term Frequency-Inverse Document Frequency)
- 문자를 숫자로 수치화하는 것
- 단어의 빈도와 역 문서 빈도를 사용해 문서 단어 행렬(DTM, Document-Term Matrix)내의 각 단어들마다 중요한 정도를 가중치로 주는 방법
