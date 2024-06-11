# Segmentation-Neural-Style-Transfer 💻 + 🎨 = ?
#### (뉴런 스타일 변화 및 특정 영역 지정 스타일 변환)

- - -

### 프로젝트 개요
- - -
### *NST 알고리즘이란?*
알고리즘은 CNN넷(일반적으로 VGG-16/19)을 사용하여 한 입력 이미지(스타일 이미지)에서 -> 다른 입력 이미지(콘텐츠 이미지)로 스타일을 전송한다.
이 프로젝트에서는 GAN을 활용한 Style Transfer을 통해 연속된 이미지의 스타일 변화를 수행하고, 특정 영역을 지정하여 스타일 변화를 한다. 


1. 스타일 이미지 + 사계절, 콘텐트 이미지 → 시간에 따라 변하는 gif 생성
2. 특정 영역(지정 영역)만 스타일 변환

   
다음과 같이 Style transfer 응용 분야 확장 총 두 가지를 수행함.


- - -
### 필요한 라이브러리 
- - - 
> *python*,  *numpy*, *os*, *argparse*, *matplotlib*, *cv2* 기타 등등...

### channels:
  - defaults
  - pytorch
    
### dependencies:
  - python=3.7.6
  - pip=20.0.2
  - matplotlib=3.1.3
  - pytorch==1.4.0
  - torchvision=0.5.0

### pip:
  - numpy==1.18.1
  - opencv-python==4.2.0.32
- - -
### 데이터 세트
- - -
직접 촬영한 8초 짜리 학교 영상을 -> 초당 프레임이 **30fps**인 **240**장의 연속된 사진들로 변환함.

### ![학교 영상](https://github.com/ryu020619/Segmentation-Neural-Style-Transfer1/blob/main/ky_school.mov) << 눌러서 원본 동영상 확인


![연속 된 사진](https://github.com/ryu020619/Segmentation-Neural-Style-Transfer1/blob/main/image.png)




=> 위 사진과 같이 content_0to59 파일 안에 저장된 60장의 사진들.

=> content_0to59, content_60to119, content_120to179, content_180to239 총 4개의 파일에 구분해둠.

- - -
### 모델 설명 - 사용한 모델의 종류 및 선택 이유
- - -

content로 사용할 연속적인 학교 이미지 중 가장 첫 번째 사진

![학교 첫 번째 이미지](https://github.com/ryu020619/Segmentation-Neural-Style-Transfer1/blob/main/frame_0000.jpg)
- - -
### 실험 결과
- - -
### 추후 개선 사항
- - -
