---
layout : single
title : "Data Manipulate"
categories : DATA
tag : [Pandas, Tidy Data, EDA]
toc : true
author_profile : false 
search : true #검색 원치 않으면 false
---

# Data Manipulate

## **개요**

* Data Manipulation이란?
  * 데이터의 가독성을 높이고 조직적으로 만들기 위해 데이터를 변경하는 프로세스
  * 데이터 분석을 용이하게 하기 위해 데이터 세트를 구조화 하는 프로세스
* 표준원칙 3가지
  1. Every column is a variable(모든 열은 변수)
  2. Every row is an observation(모든 행은 관찰값)
  3. Every cell is a single value(모든 셀은 단일값)
* Messy dataset에서 주로 발생하는 5가지 문제들
  1. Column headers are values, not variable names.(열의 header가 이름이 아닌 value값일 때)
  2. Multiple variables are stored in one column.(여러개의 변수가 하나의 열에 저장될 때)
  3. Variables are stored in both rows and columns(변수가 행과 열에 모두 저장될 때)
  4. Multiple types of observational units are stored in the same table(여러 유형의 타입이 한 개의 테이블에 존재할 때)
  5. A single observational unit is stored in multiple tables(단일 관측치가 여러 개의 테이블에 저장될 때)

## **방법**

* Pandas

  * Concat(Concatenate)

    * 데이터를 물리적으로 붙이는 것

      <center><img src="https://user-images.githubusercontent.com/81834043/162617875-6120cd39-a926-48d5-bb6f-085f8ea25b5b.png" alt="(사진2)" style="zoom:100%;"/></center>

    * Concat시 ignore_index = True로하면 index가 순차대로 데이터가 떨어짐

    * Concat시 비어있는 데이터는 NaN처리됨

  * Merge

    * 교집합을 찾아서 붙이는 것

      <center><img src="https://user-images.githubusercontent.com/81834043/162617950-91d9c822-0b58-48e5-a72a-377d6a6dd517.png" alt="(사진2)" style="zoom:100%;"/></center>

    * Merge 조건 / Default는 INNER

      <center><img src="https://user-images.githubusercontent.com/81834043/162617982-c7874765-9c8a-4fde-a223-7efc73c517ed.png" alt="(사진2)" style="zoom:80%;"/></center>

      * Outer과 Concat이 다른 부분은/ Merge는 중복된 부분은 다시 표현되지 않음
      * on = ‘a’ 의 조건은 : on에 적혀있는 데이터는 생기고, 그 이후의 데이터들은 따로따로 데이터를 가지고 온다

  * Conditioning

    * 원하는 조건에 맞는 데이터 추출시
    * `&(and)` 와 `|(or)`를 사용하여 여러개의 condition을 동시에 조절하여 사용

  * isin

    * 숫자형(numerical) 값을 기준으로 사용하는 것이 아닌, 범주형(categorical)데이터를 기준으로 조건분류 할 때 사용

    * 예시

      * ```python
        df_subset[df_subset['테마'].isin(['주류'])] 
        ```

      * ```python
        df[(df['테마'] == '주류')]
        ```

  * Groupby

    * 특정 조건 기준으로 데이터 값 분류할 때 사용

    * 예시

      ```python
      df_subset.groupby('테마').mean()
      ```

* Tidy Data

  * 데이터 분류시 가독성이 좋은 Data를 Tidy Data라고 부름 / 반대되는 말은 Wide Data(=long-form)

  * 좌측이 wide data / 우측이 Tidy Data

    * 'Make it tidy'라고 표현함

    <center><img src="https://d33wubrfki0l68.cloudfront.net/f6fca537e77896868fedcd85d9d01031930d76c9/637d9/images/tidy-17.png" alt="(사진2)" style="zoom:80%;"/></center>

  * 방법

    * melt()  / .pivot_table()

      <center><img src="https://user-images.githubusercontent.com/81834043/162618520-38ccb4a3-49f9-4702-abab-47c457afa788.png" alt="(사진2)" style="zoom:100%;"/></center>

    

    * Melt()사용 예시

      <center><img src="https://camo.githubusercontent.com/b2452a2716782e140ab9726873d18df3c801bf1ec979557e0f12f30e7132b620/68747470733a2f2f70616e6461732e7079646174612e6f72672f70616e6461732d646f63732f737461626c652f5f696d616765732f726573686170696e675f6d656c742e706e67" alt="(사진2)" style="zoom:100%;"/></center>

      * tidy 는 **한 행에, 한 observation**
      * 누가(`id`), 어떤 feature 값을 가지는지(`value`) **Column**을 지정해주면 됨
      * 이를 `melt`에 표현



출처 : https://cran.r-project.org/web/packages/tidyr/vignettes/tidy-data.html