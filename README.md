# 뮤지컬 포스터 멀티모달 딥러닝 흥행예측 
멀티모달 딥러닝 기반 뮤지컬 흥행 예측

## 📌 프로젝트 소개
2022 KOPIS 빅데이터 공모전 참여 <br>
[공모전 소개 링크](https://www.kopis.or.kr/por/cs/notice/csNoticeListView.do?ntt_id=2455&listCurPage=1&srchType=subject&srchText=%EA%B3%B5%EB%AA%A8%EC%A0%84&menuId=MNU_000104) <br><br>
공연 정보 데이터(KOPIS 제공) 과 뮤지컬 포스터 이미지 데이터를 활용한 멀티모달 딥러닝 흥행 예측 프로젝트 입니다.
## ⏱️ 개발 기간
총 기간 : 22.08.01 ~ 22.10.19

기획서 제출 : ~22.08.25 <br>
1차 서류심사 : 22.08.26 ~ 22.08.31<br>
1차 합격발표 : 22.09.01<br> 18팀 선정
1차 멘토링 : 22.09.20<br>
2차 발표심사 : 22.10.19<br>


## 🙋 멤버 구성
 - 김단은 - 데이터 수집, 전처리, 모델링, 발표
 - 이지현 - 데이터 수집, 전처리, 모델링, PPT제작
 - 박초은 - 데이터 수집, 전처리, 모델링, 발표

## 📌 프로젝트 내용

### [프로젝트 소개 PPT 링크](https://github.com/dannxdr/2022_kopis-multimodal_project/blob/main/ppt/%5B%EB%94%A5%EC%86%9C%5D%20%EB%AE%A4%EC%A7%80%EC%BB%AC%20%EB%A9%80%ED%8B%B0%EB%AA%A8%EB%8B%AC%20%EB%94%A5%EB%9F%AC%EB%8B%9D%20%ED%9D%A5%ED%96%89%20%EC%98%88%EC%B8%A1.pdf)

### 1. 데이터 수집 

(1) 이미지 데이터 수집
  - KOPIS OPEN API를 통해 데이터 수집
  - 2020~2022 상영한 뮤지컬 크롤링
  - 포스터 이미지가 없는 뮤지컬 제거

(2) 뮤지컬 배우, 제작사, 제작지 순위 데이터
  - PLAYDB에서 제작사, 제작진, 뮤지컬 배우 크롤링

### 2. 데이터 전처리
  - 제공 데이터에는 식별화 되어 있어 실제 공연코드와 상이함
  - Kopis api에서 추출한 ‘공연시작일자’, ‘공연종료일자’, ‘소요시간’, ‘관람연령’ 등을 토대로 식별화된 제공 데이터들와 실제 공연코드 결합.
  - 총 3093개의 데이터 중에서 중복 공연코드는 삭제 후 2307개의 데이터 활용
  - 레이블은 점유율을 고려한 판매 좌석수/총 좌석 수, 50%를 넘은 경우 흥행 성공:1, 흥행 실패:0으로 레이블 부여
  
### 3. 연구 과정

##### 모델링
  - 정형데이터 : XGBOOST 사용, 정확도 0.82
  - 이미지 데이터 : VGG-16 사용, 정확도 0.76

  
### 4. 연구결과
##### 두 모델을 합치기 위해 stacking 앙상블 기법 사용
  XGBOOST + VGG-16 ensamble 정확도 : 0.83
 
 (수정 필요)
##### 모델 예측결과 시각화
<img src="https://user-images.githubusercontent.com/80569773/236421530-00f15756-8be1-4457-9583-741a4a5ca2a3.png" width="600" height="350"/>


## 📚 skills
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=Python&logoColor=yellow"> <img src="https://img.shields.io/badge/keras-D00000?style=for-the-badge&logo=keras&logoColor=white"> <img src="https://img.shields.io/badge/tensorflow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white"> <img src="https://img.shields.io/badge/pytorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white"> 
