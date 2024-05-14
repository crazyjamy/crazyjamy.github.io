---
layout: post
title: "Barcode Scanner App"
date: 2020-03-31 17:24:00
image: 'https://github.com/crazyjamy/crazyjamy.github.io/blob/master/_images/_thumbnail/qrscanner.png?raw=true'
description: Wi-Fi 비밀번호를 QR 코드로 전달해보는 건 어떨까요?
category: 'UI/UX'
tags:
- Projects
twitter_text: QR 스캐너 애플리케이션
introduction: QR 스캐너 애플리케이션
---

## 0.1 Version

### DESCRIPTION 
2018년 여름, 우리 팀은 사내 앱을 개발하는 과정에서 QR 스캔 기능이 필요하다는 판단을 하고 개발이 진행되었습니다. 

### GOALS
- 빠른 QR 인식 
- 편한 UI
  
### SCANNING A QR CODE
<img src="https://github.com/crazyjamy/crazyjamy.github.io/blob/master/_images/_post/qrscanner/Prototype_QR_Scanner_scanning_360-628.gif?raw=true" alt="QR Scan" style="border: 1px solid #e1e1e1; border-radius: 10px;">

### SCAN ANIMATION
<img src="https://user-images.githubusercontent.com/29529125/77987124-ec2be180-7353-11ea-97c4-a6fbae1284a5.gif" alt="QR Scan" style="border: 1px solid #e1e1e1; border-radius: 10px;">
ℹ[URL](https://lottiefiles.com/18169-simple-scan-animation)

### QR CODE GENERATION
![Qr Create](https://github.com/crazyjamy/crazyjamy.github.io/blob/master/_images/_post/qrscanner/Prototype_QR_Scanner_create_360-628.gif?raw=true)
QR 제작 시에는 특별한 텍스트 제한은 없지만, 과부하나 기타 오류를 방지하기 위해 1000자로 제한하여 진행했습니다.



## 0.2 Version

### DESCRIPTION 
0.1 버전을 고도화하기 위해 아래의 개선 사항을 목표로 0.2 버전을 개발하게 되었습니다.

### GOALS
- 스캔 가능한 바코드의 종류 추가
- 제작 가능한 QR의 종류 추가
- 입력창 UI 개선


### ICONS
![추가되는 바코드 종류에 따른 Icons](https://user-images.githubusercontent.com/29529125/77995525-e986b780-7366-11ea-8872-8ec16e1dc849.png)

### UI
#### Tutorial
<img src="https://github.com/crazyjamy/crazyjamy.github.io/blob/master/_images/_post/qrscanner/img_tutorial.png?raw=true" alt="Tutorial" width="360">
#### QR Code Generation List
<img src="https://github.com/crazyjamy/crazyjamy.github.io/blob/master/_images/_post/qrscanner/img_createlist.png?raw=true" alt="QRCodeGeneration List" width="360">
#### QR Code Generation
<img src="https://github.com/crazyjamy/crazyjamy.github.io/blob/master/_images/_post/qrscanner/Prototype_QR_Scanner_generate_qr_code_vs2.gif?raw=true" alt="QRCodeGeneration" width="360" style="border: 1px solid #e1e1e1; border-radius: 10px;">
#### Setting
<img src="https://github.com/crazyjamy/crazyjamy.github.io/blob/master/_images/_post/qrscanner/img_setting.png?raw=true" alt="Setting" width="360">


## URL
[다운로드](https://play.google.com/store/apps/details?id=io.jmobile.jmscanner)


## REFERENCE
- [나무위키-바코드](https://namu.wiki/w/%EB%B0%94%EC%BD%94%EB%93%9C)
- [머테리얼-가이드](https://material.io/components/app-bars-bottom/)
- [하단 앱바](https://material.io/components/app-bars-bottom/#anatomy)
- [바코드의종류](https://docs.google.com/spreadsheets/d/12QsEy9Q259WckKjOmFr9uuO6wFndcBunB7rJhQDl1ak/edit?usp=sharing)
