# 채무 불이행 여부 예측해보기

## 💻 프로젝트 소개

[채무 불이행 예측](https://github.com/hwon-n/section2_project) 프로젝트에 많은 아쉬움을 느껴서 처음부터 다시 해보려는 마음으로 시작한 프로젝트입니다. 

<br />


## 🎮 개발 기간

22.02.15 - 22.02.25

<br />

## 🛠 사용 툴

* Colab
* Python
  * sklearn
  * pandas
  * eli5
  * yellowbrick

<br />

  
## 🔎 기존 프로젝트와의 차이점


### 데이터 전처리

기존 프로젝트에서 전처리는 범위가 넓은 지역 카테고리만 North State / Other State로 나누어서 해주었습니다. 

이번 프로젝트에서는 2가지로 나누었던 지역을 North / South / Capital로 나눠주었습니다. 또한 집 소유 여부를 3종류에서 2종류로 줄여주었습니다. 마지막으로 지역 카테고리만큼 넓은 범위를 갖고 있던 직업 카테고리를 총 3종류(natural_sciences / liberal_arts / No_info)로 줄여주었습니다. 

<br />



### 다양한 모델들 사용
기존 프로젝트에서는 배웠던 모델들을 사용해보고자 하는게 목적이었다면, 이번 프로젝트에서는 알고는 있지만 사용해보지 않은 모델들을 위주로 사용하려고 노력했습니다. 

또한 모델 선정 기준을 `과적합 방지`에 초점을 두고 총 4가지 모델을 선정해서 성능을 비교해보았습니다. 

1. XGBClassifier
2. LightGBM
3. HistGradientBoostingClassifier
4. ExtraTreesClassifier


위의 4가지 모델 중 최종적으로 선정된 모델은 검증 스코어, f1 score, ROC/AUC score가 제일 준수하게 나온 `ExtraTreesClassifier`입니다. 


<br />

  
## ✏ 프로젝트 결과



