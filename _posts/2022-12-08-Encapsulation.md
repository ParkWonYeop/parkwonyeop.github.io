---
layout: post
read_time: true
show_date: true
title: 캡슐화란?
date: "2022-12-08 18:23:20"
description: 캡슐화에 대해서 알아보자
tags:
  - Encapsulation
author: ParkWonyeop
published: true
img: ":title.png"
category: theory
---
## 서론

저번에 객체지향을 개발할때 신경써야하는 요소 중 추상화에 대해서 알아봤다.  
오늘은 또 다른 요소인 캡슐화에 대해서 알아보자  

## 캡슐화란?

캡슐화는 실제로 구현되는 부분을 외부에 드러나지 않도록 캡슐로 감싸 이용방법만 알려주는 것을 뜻한다.  
변수와 함수를 특정 역할에 따라 묶고, 외부에서 데이터에 직접적으로 접근할 수 없고, 함수를 통해 간접적으로만 접근할 수 있게 하는 것이 캡슐화이다.  

## 왜 해야할까?

코드의 중복을 피할 수 있기때문이다.  
객체 내부의 변수를 직접적으로 불러와 계산을 할 경우, 수정사항이 발생했을 떄 계산한 모든 코드를 수정해줘야한다.  
하지만 함수를 통해 접근할 경우 함수하나만 수정해주면 되기때문에 코드의 중복을 피하는 것이 중요하다.  

또한 동작방식을 외부에서 알 필요가 없어진다.  
위와 마찬가지로 객체를 직접적으로 접근하면 모든 코드에 그 객체를 계산하는 코드를 추가해야한다.  
이 과정에서 실수가 나면 전혀 다른 결과값이 나오게된다.  
하지만 캡슐화를 하여 함수에서 가져오게되면 다른 코드는 그 객체를 계산하는 코드를 알필요없이 객체의 함수만 호출하여 사용하면된다.  


## 마치며

캡슐화를 하면 코드의 오류를 줄이고 가독성이 증가하여 더 좋은 코드를 짤 수 있게 된다.  
캡슐화 외에도 다른 개념도 많으니 찾아보고 숙지해두는 것이 좋다.  