# 머신러닝 문제해결 전략 체크리스트 (이 순서로 해보자)

<br>

## 1. 탐색적 데이터 분석 (EDA)

<br>

### 데이터 구조 탐색
- [ ] 파일별 용도 파악  
- [ ] 데이터 양 확인 (레코드 수, 피처 수, 전체 용량 등)  
- [ ] 피처 이해  
  - [ ] 이름, 의미  
  - [ ] 데이터 타입  
  - [ ] 결측값 개수  
  - [ ] 고윳값 개수  
  - [ ] 실제값 확인  
  - [ ] 데이터 종류 파악  
- [ ] 훈련 데이터와 테스트 데이터 차이 분석  
- [ ] 타깃값 정의 (예측 대상 확인)  

### 데이터 시각화
- [ ] 효과적인 시각화를 위한 피처 엔지니어링 (필요 시)  
- [ ] 수치형 데이터 시각화  
  - [ ] 히스토그램  
  - [ ] 커널 밀도 추정 (KDE)  
  - [ ] 분포도  
  - [ ] 러그플롯  
- [ ] 범주형 데이터 시각화  
  - [ ] 막대 그래프  
  - [ ] 포인트플롯  
  - [ ] 박스플롯  
  - [ ] 바이올린플롯  
  - [ ] 카운트플롯  
- [ ] 피처 간 관계 시각화  
  - [ ] 히트맵  
  - [ ] 라인플롯  
  - [ ] 산점도  
  - [ ] 산점도 + 회귀선  
- [ ] 피처 파악 및 처리  
  - [ ] 추가할 피처  
  - [ ] 제거할 피처  
  - [ ] 피처별 인코딩 전략  
- [ ] 이상치 파악 및 처리  
  - [ ] 피처별 이상치 탐지 및 대응 전략  

<br>

## 2. 베이스라인 모델 구축

### 준비하기
- [ ] 데이터 불러오기  
- [ ] 기본적인 피처 엔지니어링 (필요 시)  
- [ ] 평가지표 계산 함수 구현  

### 모델 훈련
- [ ] 모델 객체 생성  
- [ ] 훈련 실행  

### 성능 검증
- [ ] 예측 수행 (검증 데이터 사용)  
- [ ] 평가 지표 계산  

### 예측 및 결과 제출
- [ ] 테스트 데이터로 최종 예측  
- [ ] 제출 파일 생성  
- [ ] 제출 완료  

<br>

## 3. 성능 개선

### 피처 엔지니어링
- [ ] 이상치 제거  
- [ ] 결측값 처리  
- [ ] 데이터 인코딩  
- [ ] 데이터 타입 변경  
- [ ] 파생 피처 생성  
- [ ] 시차 피처 생성 (시계열 전용)  
- [ ] 피처 스케일링  
- [ ] 피처명 한글화  
- [ ] 메모리 최적화를 위한 다운캐스팅  
- [ ] 새로운 피처 조합 생성  
- [ ] 불필요한 피처 제거  
- [ ] 기타 특이 피처 생성  

### 모델 훈련 + 하이퍼파라미터 튜닝
- [ ] 하이퍼파라미터 의미 파악  
- [ ] 하이퍼파라미터 선별  
  - [ ] 최적화 대상 파라미터  
  - [ ] 고정값 설정 파라미터  
- [ ] 탐색 범위 설정  
- [ ] 최적화 기법 선택  
  - [ ] Grid Search  
  - [ ] Bayesian Optimization  
  - [ ] OOF (Out-of-Fold) 예측 등  
- [ ] 튜닝 모델 생성 및 학습  

### 성능 검증
- [ ] 검증 데이터로 예측 수행  
- [ ] 성능 평가 (정확도, F1, ROC-AUC 등)  

<br>

> 참고: 이 체크리스트는 『머신러닝 딥러닝 문제해결 전략』에서 발췌하였습니다.
