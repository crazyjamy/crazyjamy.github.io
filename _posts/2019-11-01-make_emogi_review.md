---
layout: post
title: "Emogi"
date: 2019-11-01 17:24:00
image: 'https://user-images.githubusercontent.com/29529125/67750261-38f05100-fa72-11e9-9c59-d39cfaaff881.png'
description: 꿀렁이는 몽글이와의 인연
category: 'Today I Make'
tags:
- TIM
twitter_text: Emogi 제작기
introduction: 꿀렁이는 몽글이와의 인연
---


## 나의 허덕임 + 하소연 

진짜 애증하던 작업이기에 단순 모션일지라도 제작기를 쓰게되었다. 
나는 Still 이미지, 움직이지 않은 이미지로 디자이너 생을 버텨왔다. 그냥, 변명을 하자면  에펙(AFTER EFFECTS)을 제대로 할 줄 몰랐다. 
그러다가 어느 순간에 모션이 유행 되었고, 시간이 지남에 따라 벡터(SVG)에 모션을 입히는 시대가 서서히 다가왔다. 이제는 안할 수가 없게 되었다. 
사람은 적응의 동물이라고. 모르는 것에 배움을 갈구 한다고. 어찌어찌 계속해서 연습하다보니, 재미를 느끼고 알게 되었다. 🥵 
세상의 천재들은 왜 이렇게 많은지, 모션 같은 것들은 앱의 용량을 키운다고 피해 왔었는데, 이제는 용량도 별로 안든다고 한다. 세상에, 놀라워라 😑
나에게는 사실 애니메이션이 낯선 것은 아니였다. 그냥 새로운 툴에 겁이 낫던 것일까? 아니면 대학 때 한땀 한땀 그렸던 [애니메이션](https://www.behance.net/gallery/38248591/Moments-40sec-animation-video-l-2012) 에 대한 힘듬 때문에 겁이 났던 것일까 ?

## SNS 컨텐츠 제작썰 👾

제품에 관련된 피드백을 요청하는 컨텐츠 올리는 기회가 생기는 날이였다. 
때는 바야흐로 페북의 이모지가 한창 나오고 움직이는 이모티콘들이 쏟아져 나오는 시기 였다. 가장 충격을 주었던 페이스북 이모지, 당연히 파보고 싶고 똑같이 만들어보고 싶었다. 

👉 레퍼런스
![Facebook Emogi](https://user-images.githubusercontent.com/29529125/67752723-d3eb2a00-fa76-11e9-8c94-bf500485531a.jpg)

☝️스케치부터 시작하고,
![스케치](https://user-images.githubusercontent.com/29529125/67752728-db123800-fa76-11e9-8d4f-31d7ec7feb1c.png)

✌️모션을 입혔고,
![모션 입힌 후](https://user-images.githubusercontent.com/29529125/67749411-78b63900-fa70-11e9-80db-95a34baa5756.gif)

🤘다듬어서 목업에 작업하여 올렸다. 
![당시 올렸던 컨텐츠](https://user-images.githubusercontent.com/29529125/67750054-c1babd00-fa71-11e9-8806-7c7d92ad2411.gif)

## SVG(path) 기반의 모션에 대한 나의 생각

백터에 애니메이션 입히는 기술 중 하나인 [Shapeshifter](https://github.com/alexjlockwood/ShapeShifter) 는 모든 모션들이 다 가능한것도 아니고 path 기반의 morphing animation 정도가 가능한 기술이다. 
이 때까지만 해도 Shapeshifter 만의 유일한 벡터를 코드로 구현 할 수 있다고 생각해서 화려한 모션이 입혀진 이모티콘은 다 GIF 라고 생각 했던 것 같다.
그러다가 [Lottie](https://lottiefiles.com/) 가 나오면서  에펙으로 만든 애니메이션을 json으로 변환해주는 기술이 나오게 되었다. 많은 사람들이 Lottie를 사용하면서, 무수히 모션이 낑겨 넣어진, 디자인들이 쏟아져 나왔다. 
너무 과도하게 사용되어, 버벅이는 앱도 보았고, 눈을 어디다 둬야할지, 정신 없는 앱도 보았다. 

보통 	저사양 폰에서 버벅이는 경우는 아래의 경우이다. (그간 ✍️ 테스트 경험에서 나오는 팁) 
+ ✅ 레이어 정리 안한 경우
+ ✅ 레이어 이름이 한글인 경우
+ ✅ 너무 많은 모션이 한 화면에 사용된 경우 

## 몽글 거리는 것에 대한 애착
나라는 사람은 완벽한 원 보단 그냥 그... 아래에 무게중심이 잡히면서 생기는 몽글한...부분에 애착이 생기는 것 같다. 그래서 아래와 같은 캐릭터를 예전부터 추구했던 것 같다. (복잡할 것 없이 뚱냥이가 왜 좋아요? 😊 이유가 마땅히 없고 외형에서 오는 무한한 끌림 아닌가.)

움직이는 것에 흥미를 느껴서 한땀, 한땀 그려서 만들었던 캐릭터였다. 
![과정](https://user-images.githubusercontent.com/29529125/68014438-f4172500-fcd2-11e9-8f28-c1d77a01ab86.jpg)

그려서 만들었던지라 개발하시는 분께도 노가다로 slice 도 하나,하나씩 저장해가며 파일도 드렸었다. 
![SLICES](https://user-images.githubusercontent.com/29529125/68014325-89fe8000-fcd2-11e9-9a1c-f67c595b8652.png)

사내 시스템 관리 앱이여서 그냥 테스트용으로 막 이런 것도 적용하는 기회가 생겨 그것도 나름 기쁨이였다. 진짜 뒷단에 보이는 디자인은 말도 안돼는 아이콘과 UI 이긴 하지만, 신입의 패기 & 무지함 이었다고 생각한다. 


+ ✅ TEST FINAL
![TESTFINAL](https://user-images.githubusercontent.com/29529125/68016006-e4014480-fcd6-11e9-850a-c326419ad19f.gif)

## Lottie 활용

+ ✅ 만들었던 애니메이션을 정리하고 다듬었다.
![과정](https://user-images.githubusercontent.com/29529125/67750187-13634780-fa72-11e9-9146-ea10959f2936.png)

+ ✅ 다듬어진 이모지
![아웃풋](https://user-images.githubusercontent.com/29529125/67749362-59b7a700-fa70-11e9-9ca3-556860b40a2d.gif)

+ 👉Love
https://lottiefiles.com/10844-love-emogi
+ 👉Fun
https://lottiefiles.com/10889-fun-emogi
+ 👉Wow
https://lottiefiles.com/10888-wow-emogi
+ 👉Sad
https://lottiefiles.com/10843-sad-emogi
+ 👉Angry
https://lottiefiles.com/11006-angry-emogi
