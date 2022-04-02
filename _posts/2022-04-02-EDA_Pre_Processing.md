---
layout : single
title : "EDA & Pre-Processing"
categories : DATA
tag : [Pandas, EDA, Data Preprocessing]
toc : true
author_profile : false 
search : true #검색 원치 않으면 false
---

# EDA and Data Preprocessing

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

    * 많은 데이터를 눈으로 확인하기 어려울 때 그림을 이용해 데이터 집합의 범위와 중앙값을 빠르게 확인할 수 있는 목적으로 사용

    * 통계적으로 이상치(Outlier) 있는지도 확인

      <img src="../images/2022-04-02-EDA_Pre_Processing/image-20220402214935555.png" alt="image-20220402214935555" style="zoom: 33%;" />

       ###### (출처 : https://leebaro.tistory.com/entry/%EB%B0%95%EC%8A%A4-%ED%94%8C%EB%A1%AFbox-plot-%EC%84%A4%EB%AA%85)

  * Stacked bar : 막대차트의 응용으로 Bar가 누적된 형태의 차트

    <img src="../images/2022-04-02-EDA_Pre_Processing/image-20220402215206037.png" alt="image-20220402215206037" style="zoom:33%;" />

    ###### (출처 : https://jessymin.github.io/python/2019/02/10/stacked_bar_chart_python.html)

  * Parallel Coordinate : 데이터의 각 행을 변수별로 선으로 매핑시켜 나타내는 방식

    <img src="../images/2022-04-02-EDA_Pre_Processing/image-20220402215421654.png" alt="image-20220402215421654" style="zoom:33%;" />

    ###### (출처 : file:///Users/jsshin/Downloads/Dialnet-AnalisisDeDatosMultivariantesConCoordenadasParalel-5897852.pdf)

  * Heatmap : 데이터의 값을 컬러로 변환시켜 열 분포 형태로 보여주어 시각적인 분석을 가능하게 하는 데이터 시각화 기법

    ​                      <img src="../images/2022-04-02-EDA_Pre_Processing/image-20220402220143118.png" alt="image-20220402220143118" style="zoom:33%;" />   

    ###### (출처 : https://rfriend.tistory.com/419)

  Continuous & Numeric : Sactter Plot

  * Scatter Plot

* Multi-Non Graphic



# 글씨크기

## 글씨크기

### 글씨크기

#### 글씨크기

##### 글씨크기

###### 글씨크기

안녕하세요

















