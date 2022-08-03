# 특기사항
- 가천대학교 의용생체공학과 재학 중 (2023.2 졸업예정)
- 2021 산림수종 데이터 온라인 해커톤 참여 은상(3위) 수상 (2021.12)
- 가천대학교 iNES Lab AI팀 학부생 연구원 (2020.12 ~ 2022.4)
- 가천대학교 중앙동아리 ATTACK 회장 (2020.9 ~ 2021.7) 및 임원 (2017.9 ~ 2018.7)
- 대한민국 공군 만기 전역
- 제 15특수임무비행단 기지방호전대 모범병사 수상 (2019년)
- 한국 의공학 전공 연합(KBESA) 기획팀 팀장 (2017.9 ~ 2018.7)

# 사용가능 언어
- Python (가장 자신있고 많이 사용해본 언어입니다.)
- C++ (진행해본 프로젝트는 없지만 수업을 통해 배워본 언어입니다.)
- 그 외.. Html, Java Script, Java, C# 등은 간단한 프로젝트를 구현하면서 조금씩 사용해보았습니다.
- 기본적으로 언어는 큰 틀에서는 비슷하고 세부적인 부분들만 바뀐다고 생각하기 때문에, 검색과 공부를 통해 잘 모르는 언어도 충분히 구현할 수 있다고 생각합니다.

# 진행해온 프로젝트
## 딥러닝
- 2021년 1학기에 머신러닝 과목을 통해서 머신러닝에 대해 배우고 구현해본 후, 2021년 2학기에 딥러닝 수업을 통해 딥러닝에 대해 배우면서 직접 구현해보았습니다.
### 숫자 데이터 분류
- 딥러닝의 기본인 Mnist 숫자 데이터를 통해 데이터를 분류하는 모델을 생성해 본 후, 직접 숫자를 쓰고 지인들을 통해 데이터를 모아서 직접 모은 데이터로 숫자를 분류하는 모델을 생성했습니다.
- 이미지의 shape이 다 달랐고 아무렇게나 크기를 변경할 경우 이미지의 손실이 큰 경우가 있어 적절한 크기로 맞춰주었습니다.
- 모델은 VGG16의 구조와 동일하게 사용하여 모델을 학습시켰습니다.
- 모델을 학습 시킨 후, 모델의 중간층의 출력을 시각화 해보는 과정을 진행해보았습니다.
- 또한, 모델의 필터와 input 이미지에 대한 모델이 지역적 특성을 잘 파악하는지 확인하기 위한 Class Activation Map(CAM)을 통해 시각화했습니다.
- 중간층의 출력 시각화  
<img src="https://user-images.githubusercontent.com/76936390/182525480-a3e2f811-6862-4c44-8ddf-ba061ab6de7d.png">  
- 필터 이미지 시각화  
<img src="https://user-images.githubusercontent.com/76936390/182525725-373fc1ad-3b6f-4364-8bf1-f21d1eb1fd7d.png">  
- Class Activation Map(CAM)  
<img src="https://user-images.githubusercontent.com/76936390/182525856-50e534f0-f5f8-4618-97a5-527191ddae49.png" width="30%">  
- 모델 예측 결과  
<img src="https://user-images.githubusercontent.com/76936390/182526119-8a0d2385-1635-4ed4-96fe-df36d02df521.png">  
- 소스코드 : [모델 학습](https://github.com/Jihwan98/2021-2/blob/main/DeepLearning/mnist_homework/HW_main_6.ipynb)
- 소스코드 : [모델 시각화](https://github.com/Jihwan98/2021-2/blob/main/DeepLearning/mnist_homework/visualizing_my_model.ipynb)

## 데이터 과학
- 데이터 과학 수업을 들으면서 수행했던 프로젝트들 입니다.
- 기본적으로 데이터 분석을 하기 위해 필요한 python의 라이브러리들에 대해서 배웠습니다.
- numpy, pandas, matplotlib 등
- 그리고 데이터 분석을 하기 위한 방법에 대해서도 배우고, 데이터 전처리의 다양한 방법들에 대해서도 배웠습니다.
### 신용등급 예측 모델 생성하기
- 신용카드 사용자의 정보들을 모은 데이터를 통해 신용등급을 예측하는 모델을 생성해보았습니다.
- 소스코드 : [신용등급 예측. 전처리부터 모델 생성까지](https://github.com/Jihwan98/2021-1/blob/master/Data_Science/midterm_final.ipynb)  
- 데이터 분석 일부 예시 (연간 소득 / 가족 규모 or 자녀의 수와 신용등급의 상관관계)  
  <img src="https://user-images.githubusercontent.com/76936390/182314147-b0697f87-e4a8-43e2-916f-feeab08340d3.png" width="50%">

### 화재발생여부 예측 
- 건물특성과 주변 환경 데이터를 통해 각 건물들의 화재발생여부를 예측하는 모델을 생성하는 것이 목표입니다.
- 소스코드 : [화재발생여부 예측. 전처리부터 모델 생성까지](https://github.com/Jihwan98/2021-1/blob/master/Data_Science/final_report.ipynb)
- 코드 설명 영상 링크 : [유튜브 링크](https://youtu.be/weMbFrKvD-8)  
- - 데이터 분석 일부 예시 (건물구조와 건물용도분류명에 따른 화재발생여부 시각화)  
  <img src="https://user-images.githubusercontent.com/76936390/182313732-94fc924a-24b3-45f7-8454-3d5e73e04408.png" width="50%">

### 코로나 확진자 수, 유동인구, 배달 횟수 데이터를 통한 가설 수립 및 시각화
- 유동인구 데이터를 통해 가설을 세운 후 시각화 해보는 작업을 진행해보았습니다.
- 코로나 발생 이후로 유동인구가 줄었을 것이라는 가설과 코로나 확진자가 많이 발생한 지역은 적게 발생한 지역에 비해 배달 건 수가 더 많이 증가할 것이라는 가설로 진행했습니다.
- 소스코드 : [유동인구 데이터를 통한 시각화](https://github.com/Jihwan98/2021-1/blob/master/Data_Science/vz_report_1.ipynb)  
- 서울 확진자 수 추이와 서울의 유동인구 데이터 시각화  
  <img src="https://user-images.githubusercontent.com/76936390/182315771-5025eeee-94cf-4792-a8ea-97158b2adc1a.png">  
- 2020년 6/30일 까지의 지역별 누적 확진자 수 시각화  
  <img src="https://user-images.githubusercontent.com/76936390/182315251-22445d41-5c52-4a6d-9d0c-c685e66d71ab.png">  
- 지역 별, 월 별 배달 횟수 시각화  
  <img src="https://user-images.githubusercontent.com/76936390/182315982-fbbc0e97-dfb5-4966-a9ce-15b5b386a4d7.png">  
  
## 파이썬 독학
- 제일 처음 파이썬을 처음 접하면서 기본적인 문법공부와 함께 간단한 프로젝트를 개인적으로 수행해보았습니다.

### 워드 클라우드 만들기  
- wordcloud 라이브러리를 이용하여 카카오톡 단톡방의 내용으로 워드 클라우드를 만들어 보았습니다.  
- 친구들과의 단톡방의 워드 클라우드 결과입니다.  
  <img src="https://user-images.githubusercontent.com/76936390/182305686-d5e49014-dacc-4576-9429-5fa910ae90a1.png" width="30%">  

### 웹 스크래핑
- BeautifulSoup과 selenium을 라이브러리를 활용하여, 검색어를 통해 기사나 이미지를 스크랩해오는 기능을 구현했습니다.
- '추석'으로 검색했을 때의 기사 스크래핑 결과입니다.  
  <img src="https://user-images.githubusercontent.com/76936390/182307303-8bb5661c-219b-43a1-a901-20e9052a2ff1.PNG" width="100%">  
  

## 아두이노와 라즈베리파이를 통한 각종 센서 제어 프로그램 작성
- 아두이노와 라즈베리파이를 통해 각종 센서 제어 프로그램을 작성했습니다.
- 초음파센서를 통한 거리측정  
  <img src="https://user-images.githubusercontent.com/76936390/182319804-eb929b56-0ca1-4f7b-932e-180d8c86c715.png" width="50%">
