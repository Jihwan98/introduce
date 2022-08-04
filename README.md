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

## 연구실
- 2020.12 ~ 2022.4 까지 가천대학교 iNES Lab AI팀 학부생 연구원으로 활동하면서 진행한 프로젝트들 입니다.
### 스마트 턴 테이블
- 스마트 턴 테이블을 제작하는 프로젝트를 진행하였습니다.
- 스마트 턴 테이블이란 특정 호출어에 반응하여 마치 사람이 고개를 돌리듯 음성이 전달되는 방향을 예측하여 그 방향으로 테이블을 돌려주는 인공지능 기반 스마트 음성 인식 테이블 입니다.
- 스마트 턴 테이블 제작 프로토타입  
  <img src="https://user-images.githubusercontent.com/76936390/182784995-09b9e007-2e53-4015-813b-7daebd1f4e54.png"><img src="https://user-images.githubusercontent.com/76936390/182788471-73dc96cf-6040-46f9-a56b-32e61ed48772.png">  

- 간단한 소개 영상 : [유튜브 링크](https://youtu.be/EHf7p45LVyM)
- 해당 프로젝트를 대표로 팀원들과 함께 만들어 나갔습니다.
- 이 기기는 코로나 시대로 집 안에서의 생활이 증가하고, 비접촉, 비대면의 사회로 변화함에 따라 이에 걸맞는 새로운 사용자 인터페이스로 사용가능할 것이라고 판단했습니다.
- 집에서 스마트 기기를 통해 레시피를 보며 요리를 하거나 운동 영상을 보며 운동을 할 때, 손을 사용할 수 없는 상황에서 화면이 잘 보이지 않을 때 유용하게 사용할 수 있을 것입니다.
- 이 기기는 라즈베리파이와 음성을 받아 들이는 원형 마이크 어레이, 서보 모터로 구성되어 있습니다.
- 해당 프로젝트를 진행하면서, 전체 시스템 코드를 구현하고 새로운 기능들을 추가하여 전체 코드를 관리 했습니다.
- 전체 코드 깃허브 링크 : [깃허브 링크](https://github.com/Jihwan98/smart_turn_table)

#### 웹사이트 제작
- 스마트 턴 테이블을 유용하게 사용하기 위해 시스템 설정을 할 수 있는 웹사이트를 제작했습니다.
- 웹사이트 캡쳐 사진, 웹사이트 : [웹사이트 링크](https://alpha-f18cd.web.app/)
  <img src="https://user-images.githubusercontent.com/76936390/182787299-56fee4bb-820c-49db-bcf5-ddb0c0220c05.png">  
- 해당 웹사이트의 디자인은 무료로 배포하고 있는 템플릿을 활용하여 수정했습니다.
- 웹사이트의 로그인과 기기 셋팅에 대한 변수값을 처리하는 것들은 firebase를 활용하여 기능구현을 완료하였습니다.
- firebase는 구글에서 웹사이트와 어플리케이션의 기능구현을 위한 api를 제공해주는 서비스입니다.
- 사이트 배포는 firebase의 hosting으로, 로그인관련 기능 구현은 authentification, 기기 셋팅에 대한 변수값 처리는 storage를 사용하여 구현했습니다.
- 또한, 해당 기능을 웹사이트에서 구현하기 위해 html, javascript, css를 활용하여 웹사이트를 완성했습니다.
- 그리고 기기 사용에 있어 wifi 정보를 연결할 수 있도록 블루투스와 소켓 통신을 통한 wifi 정보 전송 및 수신 프로그램을 구현하여 웹사이트에 첨부해두었습니다.
- wifi 정보 전송 관련 소스 코드 : [wifi 정보 전송 관련 코드 깃허브](https://github.com/Jihwan98/smart_turn_table/tree/main/bluetooth_wifi_setup)

#### 명령어 인식 모델
- 초기 명령어 인식 모델으로는 음성을 문자로 변환해주는 deepspeech를 활용하여 문자로 변환된 결과를 바탕으로 SVM을 활용해 text word detect를 진행했습니다.
- 초기 svm 모델 관련 소스 코드 : [svm 관련 코드](https://github.com/Jihwan98/smart_turn_table/blob/main/SVM/twbc.ipynb)
- 추후, deepspeech가 너무 많은 연산을 잡아 먹었고 등록되어 있지 않은 단어는 변환을 하지 못해 우리의 목적과 맞지 않아 명령어 인식 모델 개발을 진행했습니다.
- 연구실 선배의 지도하에 음성자체에서 명령어를 인식하는 인공지능 모델을 개발을 도왔습니다. 

#### 위험상황 감지 모델
- 해당 기기의 기능 중 하나로 보안모드를 구현했습니다.
- 이 보안모드의 목적은 소리를 통해 물건이 떨어지거나 깨지는 소리, 혹은 누군가 넘어지는 소리나 살려달라는 외침, 비명 소리등 수상한 소리를 감지해 예상치 못한 위험상황을 감지하여 대처할 수 있도록 하기 위함입니다.
- 이 기능을 수행하기 위해 인공지능 모델 개발을 진행했습니다.
- 이 기능은 소리 데이터 수집에 어려움이 있었고, 우리가 찾고자 하는 소리가 매우 다양하고 명확하지 않았기 때문에 이상치 탐지에 사용하는 Auto Encoder(AE)와 Variational Auto Encoder (VAE)를 사용하여 모델을 구성했습니다.
- 소스 코드 : [위험상황 탐지 모델 코드](https://github.com/Jihwan98/abnormal_sound_detect)
- 위험상황 감지 모델의 Input, Output Mel-Spectogram
  <img src="https://user-images.githubusercontent.com/76936390/182794750-f2543906-1a6a-42c1-b1e9-9e5bca646e51.png">



## 딥러닝
- 2021년 1학기에 머신러닝 과목을 통해서 머신러닝에 대해 배우고 구현해본 후, 2021년 2학기에 딥러닝 수업을 통해 딥러닝에 대해 배우면서 직접 구현해보았습니다.
### 한국 음식 분류 모델 개발
- 한국 음식 사진을 보고 분류하는 모델을 개발했습니다.
- 이 서비스는 개인의 건강관리를 보조할 수 있는 헬스케어 서비스, SNS 등에 올라오는 사진들을 인식해 태그 명을 추천해주거나, 사진들을 자동으로 분류해 해당 단어로 검색할 때 노출이 되로록 하는 서비스, 음식 사진을 찍으면 자동으로 레시피를 찾아주는 서비스 등으로 활용 가능합니다.
- 데이터는 AI HUB에서 제공해주는 한국 음식 사진 데이터를 사용했습니다.
- 모델으로는 Inception-ResNet V2를 사용했습니다.
- Grad-CAM을 통해서 모델이 사진에서 특징을 잘 파악하는지 확인해 보았습니다.
- 모델 설명  
  <img src="https://user-images.githubusercontent.com/76936390/182531130-f267abfc-4341-4a12-83fd-6e5c19d8cc04.png" width="50%">  
- Grad-CAM  
  <img src="https://user-images.githubusercontent.com/76936390/182531477-8ae96565-55ea-4ca0-9522-f8af8b49aacc.png" width="50%">  
  <img src="https://user-images.githubusercontent.com/76936390/182531567-37417878-6706-46f1-b762-089bfa127b1a.png" width="50%">  
- 소스코드 : [음식 구분 모델 구성 및 학습](https://github.com/Jihwan98/2021-2/blob/main/DeepLearning/final_project/%EB%B0%95%EC%A7%80%ED%99%98/food_v2/500_drop.ipynb)



### Chest X-ray를 통한 정상환자, 박테리아성 폐렴, 바이러스성 폐렴, 코로나바이러스에 의한 폐렴 구분하는 인공지능 모델 개발
- 코로나 바이러스가 유행하면서 실제 의료업계에서 상용화를 진행했던 Chest X-ray를 통해 코로나바이러스를 진단하는 인공지능 모델을 개발했습니다.
- 데이터는 캐글 등 인터넷에서 연구용으로 공개해둔 Chest X-ray 데이터를 활용했습니다.
- VGG16을 활용하여 각 층을 조금씩 변경해보면서 모델을 수정했습니다.
- accuracy: 0.9215
- 이미지 분석
  <img src="https://user-images.githubusercontent.com/76936390/182529327-59da8b8b-4075-492d-a90f-301d76c11ede.png">  
- 소스 코드 : [Chest X-ray 모델 구성 및 학습](https://github.com/Jihwan98/2021-2/blob/main/DeepLearning/midterm/main_7.ipynb)
### 숫자 데이터 분류
- 딥러닝의 기본인 Mnist 숫자 데이터를 통해 데이터를 분류하는 모델을 생성해 본 후, 직접 숫자를 쓰고 지인들을 통해 데이터를 모아서 직접 모은 데이터로 숫자를 분류하는 모델을 생성했습니다.
- 이미지의 shape이 다 달랐고 아무렇게나 크기를 변경할 경우 이미지의 손실이 큰 경우가 있어 적절한 크기로 맞춰주었습니다.
- 모델은 VGG16의 구조와 동일하게 사용하여 모델을 학습시켰습니다.
- 모델을 학습 시킨 후, 모델의 중간층의 출력을 시각화 해보는 과정을 진행해보았습니다.
- 또한, 모델의 필터와 input 이미지에 대한 모델이 지역적 특성을 잘 파악하는지 확인하기 위한 Grad-CAM을 통해 시각화했습니다.
- 중간층의 출력 시각화  
  <img src="https://user-images.githubusercontent.com/76936390/182525480-a3e2f811-6862-4c44-8ddf-ba061ab6de7d.png">  
- 필터 이미지 시각화  
  <img src="https://user-images.githubusercontent.com/76936390/182525725-373fc1ad-3b6f-4364-8bf1-f21d1eb1fd7d.png" width="50%">  
- Grad-CAM  
  <img src="https://user-images.githubusercontent.com/76936390/182525856-50e534f0-f5f8-4618-97a5-527191ddae49.png" width="30%">  
- 모델 예측 결과  
  <img src="https://user-images.githubusercontent.com/76936390/182526119-8a0d2385-1635-4ed4-96fe-df36d02df521.png">  
- 소스코드 : [모델 학습](https://github.com/Jihwan98/2021-2/blob/main/DeepLearning/mnist_homework/HW_main_6.ipynb)  
- 소스코드 : [모델 시각화](https://github.com/Jihwan98/2021-2/blob/main/DeepLearning/mnist_homework/visualizing_my_model.ipynb)

## 영상 처리
- 영상처리에 대한 수업을 들으면서 딥러닝에 필수적인 영상 전처리에 대해 개념을 이해하고 직접 구현해보았습니다.
### 이미지 Augmentation Tool
- 이미지를 넣어주면 자동으로 Augmentation을 해주는 Tool을 만들었습니다.
- Label 이미지를 같이 넣어주면 Label 이미지도 같이 Augmentation이 되도록 진행했습니다.
- 상하좌우 이동, 회전, 상하좌우 전환, 밝기 변환, Histogram Equalization, 색상변경 등등을 옵션으로 받아 Augmentation을 해주는 GUI를 생성했습니다.
- Tool 소개
  <img src="https://user-images.githubusercontent.com/76936390/182533104-6e765a16-043b-460d-a44d-b09abbd95c73.png">  
- 일부 코드 소개
  <img src="https://user-images.githubusercontent.com/76936390/182533291-c30dc1df-4bd8-4fd3-97ee-15fc65829bf5.png">  
- Tool 실행 GUI 화면
  <img src="https://user-images.githubusercontent.com/76936390/182533444-a8e05255-33d1-40ec-9d41-7d31dea8e16e.png">  
- 소스 코드 : [GUI 실행 코드](https://github.com/Jihwan98/2021-2/tree/main/Image_Processing/final_project/IM2)

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
