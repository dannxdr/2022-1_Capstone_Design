# 🎬 멀티모달 딥러닝 기반 영화 흥행예측 
멀티모달 딥러닝 기반 영화 흥행 예측 프로젝트

# 📌 프로젝트 소개
### 교수 평가 : 최종 2위
클라우드 플랫폼 강의에서 진행한 멀티모달 딥러닝 기반 영화 흥행 프로젝트 입니다. <br><br>
[프로젝트 소개 pdf](https://github.com/dannxdr/predict_movie_success/blob/main/ppt/%EC%98%81%ED%99%94%20%ED%8F%AC%EC%8A%A4%ED%84%B0%EB%A5%BC%20%ED%99%9C%EC%9A%A9%ED%95%9C%20%EB%A9%80%ED%8B%B0%EB%AA%A8%EB%8B%AC%20%ED%9D%A5%ED%96%89%EC%98%88%EC%B8%A1.pdf) <br>

# ⏱️ 개발 기간
총 기간 : 22.03.02 ~ 22.06.20<br>

1차 중간 발표 : 22.04.18<br>
최종 발표 : 22.06.13<br>
최종 결과 : 22.06.20<br>


# 🙋 멤버 구성

<table>
  <tbody>
    <tr>
      <td align="center"><a href="https://github.com/peppermayoo"><img src="https://user-images.githubusercontent.com/80569773/236661679-c88ba1ce-a0e4-49d4-af0f-d15400ff31f7.png" width="100px;" alt=""/><br /><sub><b>이지현</b></sub></a><br /></td>
      <td align="center"><a href=""><img src="https://user-images.githubusercontent.com/80569773/236611467-a1b919b5-9aa7-46fb-b49a-49f1c37e7d04.png" width="100px;" alt=""/><br /><sub><b>김단은</b></sub></a><br /></td>
      <td align="center"><a href="https://github.com/park-cho-eun"><img src="https://user-images.githubusercontent.com/80569773/236661719-f9fac316-4eff-44cd-a5a5-d8ed428f0476.png" width="100px;" alt=""/><br /><sub><b>박초은</b></sub></a><br /></td>
    </tr>
  </tbody>
</table><br>
       
 - 이지현 - 데이터 수집, 전처리, 모델링, PPT제작
 - 김단은 - 데이터 수집, 전처리, 모델링, 발표
 - 박초은 - 데이터 수집, 전처리, 모델링, 발표

# 📌 프로젝트 내용

### 데이터 전처리

(1) 이미지 데이터 수집 및 전처리
  - MTCNN을 사용하여 포스터 이미지에서 인물 수 추출
  - PIL 라이브러리를 이용하여 포스터의 각 픽셀값을 수치화한후 평균값 사용
  - NAVER API를 이용하여 포스터 이미지에서 텍스트 추출 

(2) 텍스트 데이터 전처리
  - 홍보 문구 여부(수상내역, 유명감독,유명제작진)에 따라 변수 생성 및 전처리
(3) 레이블 분류 
  - 누적 관객수를 기준으로 흥행 여부를 -~3으로 분류

### 모델링

정형데이터
  - Random Forest Accuracy : 0.77
  - DNN Accuracy

이미지데이터<br>
- Pure Cnn Accuracy : 0.73
- VGG-16 Accuracy  : 0.77
 
  
### 결과
#### 멀티모달 딥러닝을 사용하여 DNN과 VGG-16을 결합
➡ Multimodal Deep Learning Accuracy : 0.81

# 📚 skills
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=Python&logoColor=yellow"> <img src="https://img.shields.io/badge/keras-D00000?style=for-the-badge&logo=keras&logoColor=white"> <img src="https://img.shields.io/badge/tensorflow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white">

