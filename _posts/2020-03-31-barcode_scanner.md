---
layout: post
title: "Barcode Scanner"
date: 2020-03-31 17:24:00
image: 'https://user-images.githubusercontent.com/29529125/77985224-ce0fb280-734e-11ea-9807-9eaa2bd8bb2e.png'
description: 제작기 (부제:Wi-Fi 비밀번호는 QR로 전달해보면 어떨까?)
category: 'Today I Make'
tags:
- TIM
twitter_text: Barcode Scanner 제작기
introduction: Wi-Fi 비밀번호는 QR로
---

## 들어가면서..
지난 2018년, 한 여름 8월 쯤에 우리 팀은 사내 앱 제작하면서 QR Scan을 하는 기능이 필요하게 되어 개발하게 되었다. 해당 기능을 Library로만 남기기에는 아쉬워 QR Scan 하는 앱을 만들어 보면 어떨까 해서 개발을 시작하게 되었다. 😶
처음에는 단순히 QR 스캔과 제작만 하는 앱을 만들려다가 QR에 대해 공부하면서 QR은 바코드의 한 종류 였다는 것을 알게되었다. 바코드의 역사, 종류, 음모론을 공부하게 되는데 상당히 빠져들게 되었다. 🤖알면 알수록 신비롭고 괴상한 바코드의 세계, 일본에서는 바코드 리더로 상품 바코드를 읽어들여 캐릭터 능력치를 입혀가는 미연시 게임도 있다고 할정도로 바코드로 시작하여 바코드의 풀이의 끝은 무궁무진했다. 

## 목적
우리의 목적은 2가지 였다.
- ✅빠르게 QR을 인식시키고 
- ✅재미있게 QR을 만들어보자 였다.

그 당시 힙했다는 [하단 앱바](https://material.io/components/app-bars-bottom/#anatomy)를 활용하려고 꽤나 애를 썼다.😄 개발하시던분도 나도 정말 고생이 많았다. 나는 QR 정보를 입력하면서 실시간에 QR의 모양이 바뀌어 나간다면 사용자들이 흔하지만 낫설게 느낀 QR을 조금 더 재밌게 만들지 않을까에 꽂혔던것 같다.
그 때는 와 나 천재네? 이랬지만, 지금은 여래개의 QR을 입력해야하는 경우라면 사실 웹이나 다른 UI가 나을지도 모른다는 생각은 2년이 지난 지금 들긴한다. 🤡

### 텍스트 입력창의 간단한 Prototype
가장 고민을 많이 했던 부분 중 하나는 입력창을 위(Prototype1)에 두느냐 아래(Prototype2)에 두느냐였다. 테스트 결과 텍스트가 넘칠시에 뒷단에서 보이는 QR 이미지 생성하는 부분을 실시간으로 보기에는 힘들 것 같다는 의견도 있었고, 키패드 위에 텍스트 입력창을 두는게 시선처리가 편하다는 의견도 있어 입력창은 아래에 두었다.

#### 👉Prototype1 
![Prototype1](https://user-images.githubusercontent.com/29529125/77986816-00231380-7353-11ea-83c8-47a591ec18d2.gif)

#### 👉Prototype2
![Prototype2](https://user-images.githubusercontent.com/29529125/77986163-63ac4180-7351-11ea-93fc-ca484fe5d82c.gif)

#### 👉스캔시 사용된 애니메이션 
ℹ︎[lottie 경로](https://lottiefiles.com/18169-simple-scan-animation)

QR의 사각형 모양을 본따 스캔이 잘되고 있는 사용자의 심리적인 인식을 심어주기 위한 소소한 애니메이션이다.
![Scanning Animation](https://user-images.githubusercontent.com/29529125/77987124-ec2be180-7353-11ea-97c4-a6fbae1284a5.gif)



## 1차 버전 완료
빠르게 스캔도 되고, 실시간으로 입력된 문구마다 변경되는 QR의 모습은 이루게 되면서 개발이 완료 되었다. 
실제 개발이 완료된 녹화 영상은 아래에 첨부하여 본다.

#### 👉QR 스캔
![QR Scan](https://user-images.githubusercontent.com/29529125/77983272-86d2f300-7349-11ea-8fa3-9ac7868f25ab.gif)

#### 👉QR 제작
QR 제작시에는 특별한 문자 제한은 없지만, 과부하나 기타 오류를 제한하기 위해서 1000자로 제한하여 진행하였었다.

![Qr Create](https://user-images.githubusercontent.com/29529125/77982474-63a74400-7347-11ea-957b-bcd08cb808a2.gif)


## QR Scanner -> Barcode Scanner 
초기버전에는 단순히 QR제작과 스캔만 되는 버전이였지만, 바코드를 더 추가하여 발전시켜보려고 노력하여 보았다. 
개선하고자 하는 3가지

- ✅스캔 가능한 바코드의 종류 추가
- ✅제작 가능한 QR의 종류 추가
- ✅입력창 UI 개선

### 바코드의 종류 
공부하면서 느낀 것은 바코드의 종류는 생각보다 많았다. 추가해 볼 만한 바코드와 데이터 타입을 엑셀로 정리하여 보았다. 많은 종류 중에 몇 개만 더 추가해볼까? 하면서 프로젝트는 조금 씩 커져갔다.
👉[바코드의종류](https://docs.google.com/spreadsheets/d/12QsEy9Q259WckKjOmFr9uuO6wFndcBunB7rJhQDl1ak/edit?usp=sharing)

#### 추가 되는 QR 데이터의 종류
- ✅이메일
- ✅URL
- ✅전화번호
- ✅연락처
- ✅와이파이

#### 추가되는 기능에 아이콘들도 한번씩 손을 보게 되었다.

![추가되는 바코드 종류에 따른 Icons](https://user-images.githubusercontent.com/29529125/77995525-e986b780-7366-11ea-8872-8ec16e1dc849.png)

### 입력창 UI 개선 
추가되는 바코드 종류에 따른 현재 적용된 입력창의 한계가 있어서 변경 하게 되었다.

#### 👉입력창이 1개인 경우
![Prototype_textInsert](https://user-images.githubusercontent.com/29529125/77997793-f60d0f00-736a-11ea-90ac-45fbd2466a8e.gif)
#### 👉입력창이 다수인 경우
![Prototype_textInsert](https://user-images.githubusercontent.com/29529125/77997819-058c5800-736b-11ea-9290-9ff1ed7c604a.gif)


#### 8.참고 문서 
- [나무위키-바코드](https://namu.wiki/w/%EB%B0%94%EC%BD%94%EB%93%9C)
