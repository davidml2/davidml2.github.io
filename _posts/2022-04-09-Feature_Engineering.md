---
layout : single
title : "Feature Engineering"
categories : DATA
tag : [Pandas, Feature Engineering, Data Preprocessing]
toc : true
author_profile : false 
search : true #검색 원치 않으면 false
---

# Feature Engineering



* Feature Engineering 이란?

  도메인 지식을 활용하고 창의성을 발휘하여, 기존 데이터셋에 존재하는 Feature들을 재조합하여 Target에 맞는 새로운 Feature를 만드는 과정

* 예시

  키와 몸무게와 나이와 성별을 알 경우에 이를 바탕으로 BMI지수라는 새로운 Feature를 만들어 내는 것

* 데이터프레임(Data Frame)이란

  * 대중적인 표형식 데이터에 대한 통계 및 시각화에 활용하는 자료구조
  * 동일한 길이를 갖는 벡터 집합
  * read.csv(), read.table()로 함수를 만들어 냄

* 유용기법

  * String Replace

  * 숫자 사용시 표현은 숫자로 되어있지만, string datatype일 때 Integer datatype으로 변경 필요

    * s.replace(',',' ')

    * ```python
      def toInt(string):
          return int(string.replace(',',''))
      ```

* Pandas datatype 형태

  <center><img src="https://user-images.githubusercontent.com/81834043/162576682-6e58e106-131e-4ae8-ab28-6ae65dda83d6.png" alt="(사진2)" style="zoom:50%;"/></center>

  

* Na,Null,NaN(Not a Number),0, Undefinded차이

  * NaN(Not a Number) : **숫자로 변환되지 않는 문자열과의 나누기 연산 등 잘못된 수식으로 인하여 발생한 값,** 프로그래밍 상 Float처리됨, boolean 형변환 결과는 false

    Na : NaN과 동일한 의미를 함(실제로 Na는 Python에는 없음,R에서만 주로 사용함)

  * Null : **비어있음을 의미하는 값(아직 정해지지 않는 값),** boolean으로 형변환이 일어나는 경우 flase가 됨

  * 0 : 숫자 0 데이터를 기입

  * Undefinded :  **비어있는 상태**, boolean으로 형변환이 일어나는 경우 false가 됨

  * None : **비존재, 비어있는 값**

<center><img src="https://user-images.githubusercontent.com/81834043/162576752-81e83963-f440-48f2-ba07-83fa7550ee9d.png" alt="(사진2)" style="zoom:50%;"/> </center>





