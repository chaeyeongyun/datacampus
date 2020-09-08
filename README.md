# 빅데이터 청년캠퍼스 2조
-----------------------
## 세탁을 위한 fashion detection
---------
* 진행기간 2020.07.17 ~ 2020.09.10
---------------------------
## 1. 개발배경
* 자취생들의 빨래에 대한 어려움
  (세탁물 물빠짐, 줄어듬 등)
* 삼성, LG 등 기업들의 AI를 이용한 자동화 세탁기 출시 트렌드
## 2. 목표
* 자취생들에게 쉽게 빨래에 대한 정보를 전달하는 서비스 개발 및 세탁 자동화 시스템 구현

## 3. 팀 소개
> 유성호
* 팀장
* 개발 환경 구축, 프로젝트 관리, 발표, 분류 모델 평가, web 구현
> 정세환
*  모델 학습 자동화, 데이터 전처리, 분류 모델 평가, web 구현
> 신동환
*  학습 데이터수집, 라벨링 ,ppt 제작
> 김가연
* 학습 데이터수집, 라벨링 ,영상 편집
> 정승연
* 모델 학습 자동화
> 윤채영
* 학습 데이터수집, 라벨링 ,ppt 제작

## 4. 시스템 사용 Tool
![dsBuffer bmp](https://user-images.githubusercontent.com/70565663/92070647-99b18e00-ede7-11ea-98c6-ddc06cb7af70.png)

## 5. 프로젝트 요약
* 공개되어있는 dataset과 crawling을 통해 의류 데이터 수집
* (시간 관계 상 상의만 진행)
* image의 상의 영역만 Boundary 처리
* 여러 deep learning model로 training 및 test 진행
* (VGG16, DenseNet, Inception V3, Inception-ResNet V2)
* accuracy 가장 높은 model로 구현(Inception V3)
* web application으로 서비스화 및 시각화
* 사용자가 사진 입력시 재질, 색, 소매길이를 인식
* 그에 맞는 세탁방법 제공

## 6. Requirement
* Keras version : 2.4.3
* Tensorflow version : 2.3.0

## 7. Code Explanation
We used google colab
* image data는 color, fabric, sleeve 3개의 category가 들어있는 image data 첨부
* image detection을 위해 필요한 pretrained model(fabric.h5, color10.h5, length.h5) 첨부

* Inferece.ipynb : optimizer 을 직접 epoch을 설정하며 구현한 model
* main.ipynb : model을 불러 시각화
* 주석을 참조해주세요
* ppt 참조
* 구현 결과 html 첨부

