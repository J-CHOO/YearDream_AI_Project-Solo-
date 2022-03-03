# YearDream_AI_Project-Solo-
p2p 대부업체의 고객 데이터를 통한 채무 불이행 여부 예측 과제 (데이터는 저작권상 공개하지 않습니다.)
  - 이어드림스쿨 AI과정 중에 진행한 프로젝트로, [AI connect](https://www.aiconnect.kr/main/competition/privateDetail/203/competitionInfo)플랫폼에서 진행한 대회입니다.
## 1. 대회설명
- 신청 기간 : ~ 1월 26일 08:59 AM
- 대회 기간 : 1월 26일 09:00 AM ~ 2월 8일 12:00 PM
- 참가 대상 : 이어드림 스쿨 수강생으로 제한
- 개인전 (팀 머지 불가)
  - p2p 대부업체의 고객 데이터를 활용한 채무 불이행 여부 예측 과제 수행
  - 본 과제는 실시간 리더보드를 운영하며, 대회 마감 후 추론에 사용한 코드 파일(.ipynb)을 대회 페이지의 '코드 공유' 탭을 통해 제출

## 2. 과제개요
- 대출자 채무 불이행 여부 예측 모델 수치 영역 | 개방형 문제 | Macro F1 score

- 문제정의
  - p2p 대부업체의 고객 데이터로부터 고객의 채무 불이행 여부에 대한 이진 분류

- 추진배경
  - 핀테크 분야 성장에 따른 금융 분야 AI 활용도 증가
  - 금융 서비스 고객의 분류를 통한 금융 시장 건전성 제고 목표

## 3. 데이터 설명
- 문제설명
  - p2p 대부업체의 고객 데이터를 통한 채무 불이행 여부 예측 과제
  - target 변수가 depvar(dependent variable)라는 이름으로 train.csv에 들어가 있음.
  - 나머지 변수들을 feature로 target 값을 예측하는 모델을 만들어 봄.

- 제출방법
  - 첨부드린 sampe_submission.csv의 answer 값을 추론 값으로 채워서 제출

## 4. 프로젝트 과정
처음 하는 프로젝트라 기본 Base라인을 최대한 활용하여, Grid_search로 각 모델별로 하이퍼 파라미터를 찾아 F1 Score를 올렸다.

1. EDA진행
2. 모델 설정 후 학습(lgbm, xgb model, RandomForestClassifier등 사용)
3. Grid_search로 여러 조합의 하이퍼파라미터를 넣어, 최적의 하이퍼 파라미터를 탐색
4. 학습 향상을 위해 앙상블 모델(stacking) 사용
5. test 데이터에 최적모델을 적용 한 후 submit 파일로 대입시킨 후 제출

## 5. 사용 스택
- 개발 환경
  - Jupyter Notebook
- 기술 및 라이브러리
  - Python, numpy, Pandas, Sklearn, Seaborn, Matplotlib, Xgboost, Lightgbm, RandomForestClassifier

### 주최
중소벤처기업진흥공단

### 주관
마인즈앤컴퍼니
