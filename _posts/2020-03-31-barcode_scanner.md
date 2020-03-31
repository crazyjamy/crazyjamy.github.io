---
layout: post
title: "Barcode Scanner"
date: 2020-03-31 17:24:00
image: 'https://user-images.githubusercontent.com/29529125/77985224-ce0fb280-734e-11ea-9807-9eaa2bd8bb2e.png'
description: Wi-Fi 비밀번호는 QR로
category: 'Today I Make'
tags:
- TIM
twitter_text: QR Scanner 제작기
introduction: Wi-Fi 비밀번호는 QR로
---

## 들어가면서..
지난 2018년, 한 여름 8월 쯤에 사내 앱 제작하면서 QR Scan을 하는 Library를 개발하게 되었다가 Library로만 남기기에는 아쉬워 Barcode Scan 하는 앱을 만들어 보면 어떨까? 해서 개발을 시작하게 되었다. 😶 더 나아가자면, 당시 지란패밀리라는 사내 공모 행사가 있어서 행사에 공모해 볼 사이드 프로젝트로 진행하여 보자는게 진짜 이유였다.
처음에는 단순히 QR 스캔과 제작만 하는 앱을 만들려다가 바코드 몇개만 더 추가해볼까? 하면서 바코드의 역사, 종류, 음모론을 공부하게 되는데 상당히 빠져들게 되었다. 🤖
알면 알수록 신비롭고 괴상한 바코드의 세계, 일본에서는 바코드 리더로 상품 바코드를 읽어들여 캐릭터 능력치를 입혀가는 미연시 게임도 있다고 할정도로 바코드로 시작하여 바코드의 풀이의 끝은 무궁무진했다. 

## 초기 버전 
우리의 목적은 빠르게 QR을 인식시키고, 재미있게 QR을 만들어보자 였다.
그 당시 힙했다는 [하단 앱바](https://material.io/components/app-bars-bottom/#anatomy)를 활용하려고 꽤나 애를 썼다.😄 개발하시던분도 나도 정말 고생이 많았다.
그 당시 나는 QR 정보를 입력하면서 실시간에 QR의 모양이 바뀌어 나간다면 사용자들이 흔하지만 낫설게 느낀 QR을 조금 더 재밌게 만들지 않을까에 꽂혔던것 같다.
그 때는 와 나 천재네? 이랬지만, 지금은 여래개의 QR을 입력해야하는 경우라면 사실 웹이나 다른 UI가 나을지도 모른다는 생각은 2년이 지난 지금 들긴한다. 🤡

👉QR 스캔
![QR Scan](https://user-images.githubusercontent.com/29529125/77983272-86d2f300-7349-11ea-8fa3-9ac7868f25ab.gif)

👉QR 제작
QR 제작시에는 특별한 문자 제한은 없지만, 과부하나 기타 오류를 제한하기 위해서 1000자로 제한하여 진행하였었다.

![Qr Create](https://user-images.githubusercontent.com/29529125/77982474-63a74400-7347-11ea-957b-bcd08cb808a2.gif)

👉스캔시 사용된 애니메이션 
![Scanning Animation]()

## 바코드의 종류 
초기버전에는 단순히 QR제작과 스캔만 되는 버전이였지만, 바코드를 더 추가하여 발전시켜보려고 노력하여 보았다. 바코드의 종류는 생각보다 많았다. 
추가해볼만한 바코드와 데이터 타입을 엑셀로 정리하여 보았다. 
👉[바코드의종류](https://docs.google.com/spreadsheets/d/12QsEy9Q259WckKjOmFr9uuO6wFndcBunB7rJhQDl1ak/edit?usp=sharing)




#### 8.참고 문서 
- [나무위키-바코드](https://namu.wiki/w/%EB%B0%94%EC%BD%94%EB%93%9C)
