Resume
================
양정열

<passionyang16@gmail.com>

010-2811-6370

데이터 분석 관련 이력서입니다.

언어: Python, R


# Projects

데이터 분석 관련 프로젝트 리스트입니다.

## 3줄 요약 웹사이트

[Github Link](https://github.com/passionyang16/3-lines-summary)

사용언어: Python

KoBERT를 활용한 문서 추출 요약 웹 구현

- Pytorch로 직접 Transformer 모델 구현
- Google Colab TPU 사용하여 학습
- Flask와 Node.js를 활용하여 웹 


## 주식 자동 트레이딩 프로그램

[Github Link](https://github.com/passionyang16/stock_trading)

사용 언어: Python

Version 1)

NLP를 활용하여 테마주를 미리 사서 정해진 밴드에 맞춰 매매

- 네이버 뉴스에 테마, 뉴스, 종목 크롤링
- KoBert로 Tokenize, Word2Vec으로 Vectorize
- Stopwords와 정규표현식으로 meaningless한 데이터 전처리
- 뉴스 vector와 테마 vector를 비교해 코사인 유사도가 가장 높ㅇ은 테마 선정
- 리스크를 줄이기 위해 +5% 상한선, -5% 하한선의 밴드를 설정하고, 해당 밴드를 벗어나면 매도

Version 2)

변동성이 큰 상한가 다음날 종목을 매매

- 대신증권 크레온 API로 2년치 상한가 다음날 종목 데이터 매분마다 수집
- 몇시 몇분 매수, 몇시 몇분 매도가 가장 큰 수익률을 가져다주는지 정밀한 데이터 분석 진행
- 대신증권 크레온 API request / response를 통해 주식 자동 트레이딩 프로그램 완성


## 데이터사이언스입문 수업 부동산 가격 예측 프로젝트

[Github Link](https://github.com/passionyang16/ProjectCasa)

사용 언어: Python

비지도 학습과 시계열 분석을 활용한 부동산 가격 예측

  - 네이버 부동한 크롤링을 통해 서울 내 부동산 데이터 수집

  - 비슷한 특징을 가진 아프트끼리 K-Prototype을 통한 군집화

  - ARIMA 시계열 분석을 통한 아파트 가격 예측 (결측치는 동일 군집에서 비슷한 아파트의 가격으로 대체)

## YBIGTA 데이콘 천체유형 분류 대회 머신러닝 프로젝트

[Github Link](https://github.com/passionyang16/ProjectCelestial)

사용 언어: Python

지도 학습을 활용한 천체 유형 분류 분석

  - EDA를 통한 데이터 전처리, scikit learn 활용

  - 분류 분석에 유용한 앙상블 기법 중 XgBoost, LightGBM 사용

  - 데이터 마이닝 관련 필요한 과정 포함



# 기타

## Algorithm Practice

[Github Link](https://github.com/passionyang16/algorithm)

사용 언어: Python

기초적인 컴퓨터 공학 자료구조와 알고리즘를 익히기 위한 문제 풀이

  - 백준 / 프로그래머스

## R Machine Learning Codebook

[Github Link](https://github.com/passionyang16/r_codebook)

사용 언어: R

머신 러닝에 필요한 다양한 기법들을 쉽게 사용하기 위한 R Codebook


# Courses

응용통계학과를 전공으로 하면서 수강했던 과목들 리스트입니다.

  - 통계학입문
  - 통계방법론
  - 미분적분학
  - 선형대수
  - R과 파이썬 프로그래밍
  - 수리통계학 1, 2
  - 회귀분석
  - 확률 과정
  - 데이터 마이닝
  - 딥러닝
  - 데이터 사이언스 입문
  - 금융공학의 이해
  - 시계열 분석


# Coming Soon

## 맞춤형 정보성 뉴스 알림 앱, 뉴스보이

사용언어: Python, Java / Spring, Flutter / Dart

뉴스보이는 키워드 검색 시 휴대폰에 도배되는 중복되고 자극적인 뉴스, 가뜩이나 바쁜 현대인에게 너무나도 긴 뉴스의 내용, 찾기 어려운 본인에게 정말 필요한 뉴스 등의 문제를 해결하기 위해 "중복이 제거되고 3줄로 요약된 뉴스만을 보여주며, 사용자가 구독한 키워드에 해당하는 뉴스를 푸시 알림으로 제공해주는 앱"이다.

- 자연어로 이루어진 뉴스 기사를 Sent2Vec 벡터화 후, 코사인 유사도를 기준 DBSCAN 클러스터링 기법으로 비슷한 뉴스들 그룹화
- 해당 그룹에 있는 뉴스 중 가장 중립적이고 정보성이 많은 뉴스만 대표뉴스로 선정, 나머지 뉴스들은 제거
- 비슷한 뉴스가 가장 많이 모인 그룹 내림차순 정렬, 순서대로 당일 이슈가 많은 것으로 판단, 앱 메인 화면 상단 10개의 TOP 뉴스를 슬라이드 형태로 제공
- 앱 메인 화면 하단 사용자 검색 및 뉴스 클릭 로그를 기반으로 한 뉴스를 리스트 형태로 추천
- NLP 모듈 카카오 PORORO를 활용하여 미리 학습된 BERT로 화면 내 특정 뉴스 클릭 시 전체 화면으로 메인 이미지, 3줄 요약된 뉴스 내용, 구독할 수 있는 고유명사 기반 키워드 등제공
- 구독 화면 상단 사용자가 구독한 키워드들이 각각 버튼 형식으로 되어, 해당 버튼 클릭시 관련 기사가 리스트 형태로 제공.
- 구독한 키워드 중 새로운 뉴스가 업데이트 되면 사용자에게 푸시 알림으로 해당 내용을 전달 (Firebase 활용)
- Algolia를 활용한 검색 기능 탑재
