---
layout : single
title : "EDA & Pre-Processing"
categories : DATA
tag : [Pandas, EDA, Data Preprocessing]
toc : true
author_profile : false 
search : true #검색 원치 않으면 false
---

# EDA(Exploratory Data Analysis) and Data Preprocessing

## EDA(Exploratory DATA Analysis)

### 개요

* EDA란?

  데이터 분석에 있어서 초기 분석의 단계이며, 데이터 분석 전체 프로세스 중에 7 ~ 80% 시간을 소모할 만큼 중요한 부분입니다.

* 내용

  * 패턴발견 : 시각화 도구 사용
  * 데이터 특성 발견
  * 가설 검정 : 통계, 그래픽, 시각적 표현 등을 사용

* 종류

  * Graphic : 그림,차트,시각적 요소를 통해 데이터를 확인
  * Non-Graphic : Summary Statistics를 통해 데이터를 확인

* Target

  * Univariate
  * Multi-Variate : 여러 변수들간의 관계를 보는 것이 주요 목적

### 구분

EDA의 종류와 Target을 조합하여 아래와 같이 구분합니다.

* Uni-Graphic

  Histogram, Pie chart, Stem-leaf plot, Boxplot, QQplot, Binning, Tabulation 등을 사용합니다.

  * Histogram : 순서형 자료와 수치형 자료를 도수분포표를 이용해서 그래프 형태로 나타낸 것
  * Pie chart : 파이형태로 명목자료를 그래프로 표시하는 방법으로, 각 계급의 비율을 중심으로 볼 때 많이 사용
  * Stem-leaf plot : 
    * Histogram을 옆으로 돌려 높은 것과 같은 숫자형 자료에 사용
    * Histogram과 달리 정보손실이 없음, 각 자료의 값을 알 수 있어 추가 정보를 더 얻을 수 있음
    * 줄기(Stem)과 잎(Leaf)로 구성
      * 한 줄기에 0에서 9까지의 잎이 가능
  * Boxplot : 막대그림의 명목자료를 그래프로 표시하는 방법으로, 순위를 정할 때 많이 사용
  * QQplot : 데이터의 분포와 이론상 분포가 잘 이치하는지 확인
  * Bining : Data를 bining한다 라고 부르기도 하는데, 이는 정의된 기준에 따라 각각의 개별적인 데이터값을 특정한 bin(구간, interval) 또는 group으로 묶는 과정을 의미
  * Tabulation : 범주형 변수일 경우 교차분석(Cross tabulations)을 사용

* Multi-Graphic

  Category & Numeric : Boxplots, Stacked bar, Parallel Coordinate, Heatmap

  * Boxplots :
  * Stacked bar :
  * Parallel Coordinate :
  * Heatmap :

  Continuous & Numeric : Sactter Plot

  * Scatter Plot

* Multi-Non Graphic



















