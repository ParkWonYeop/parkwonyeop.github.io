---
layout: post
read_time: true
show_date: true
title: Http Method에 대해서 알아보자
img: ":title.png"
date: "2023-04-01 18:23:20"
description: Http Method에 대해서 알아보자
tags:
  - HTTP
author: ParkWonyeop
published: true
category: web

---

## 서론

우리가 웹 통신을 할때 Get, Post 와 같이 통신 방식에 대해서 들어본적 있을 것이다.  
오늘은 Http Method의 종류와 사용용도에 대해서 알아보자.  

## Http Method란?

### Hyper Text Transfer Protocol

클라이언트와 서버가 인터넷이나 네트워크를 통해 통신하는 표준화된 방법이다.  
Http Method는 클라이언트가 서버에서 제공하는 리소스에 대해 수행하려는 작업 유형을 정의한다.  

## 종류

Http Method에는 여러가지 종류가 있다.  

1. Get  
- 클라이언트는 리소스를 수정하지 않고 서버에서 정보를 탐색할 때 사용한다.  
Get 메서드는 안전하고 멱등적이다. 즉 여러개의 동일한 요청이 단일 요청과 동일한 효과를 가져야한다.  

2. Post  
- 일반적으로 새 리소스를 만들거나 공개되면 안되는 데이터를 제출하는데 사용한다.  
Post 메서드는 멱등성이 없다. 즉, 동일한 요청을 여러개보내면 서버에 서로 다른 영향을 미칠 수 있다.  

3. Put  
- 현재 데이터를 새로운 데이터로 대체하여 서버의 리소스를 업데이트할때 사용한다.  
Get 메서드와 마찬가지로 멱등적이므로 동일한 요청을 여러 번 보내도 늘 같은 효과를 낸다.  

4. Delete  
- 서버의 데이터를 삭제할때 사용한다.  
멱증적이므로 동일한 요청을 여러번 보내도 늘 같은 결과가 나온다.  

5. Patch
- 서버의 데이터의 일부만을 수정하여 새로운 데이터로 업데이트한다.  
Put과 다른점은 서버의 데이터 전체를 바꿔치기하는 Put과는 달리 일부분만을 수정한다.  
그렇기때문에 멱등적이지 않아서 동일한 요청을 여러번 보내도 매번 결과가 다르다.  

위의 메소드들은 자주 사용하는 것들이고 아래는 자주 사용하지 않는 것들이다.  

6. Head  
- 이 메서드는 Get과 유사하지만 리소스가 아닌 헤더만 가져온다.  
클라이언트가 전체 리소스를 실제로 다운로드하지않고, 리소스가 존재하는지 확인하거나 메타데이터를 검색하는 경우에 사용한다.  
안전하고 멱등적이다.  

7. Options  
- 이 메서드는 지정된 리소스에 사용할 수 있는 통신 옵션에 대한 정보를 검색한다.  
서버가 지원하는 Http Method의 종류의 목록을 반환한다.  
안전하고 멱등적이다.  

8. Connect  
- 이 방법은 Https 연결과 함께 사용하기 위해 일반적으로 프록시 서버와 네트워크 연결을 설정하는데 사용한다.  
Connect 요청은 안전하지도 않고 멱등성 또한 없다.  

9. Trace  
- 이 메서드는 지정된 리소스에 대한 요청 및 응답 메세지의 진단 표현을 검색한다.  
안전하고 멱등적이다.  

## 마치며

요약하면 Http Method는 클라이언트가 서버에서 제공하는 리소스를 수행하는 작업을 정리한 것이다.  
각 방법은 특정 용도에 사용되며 표준화된 방법으로 인터넷이나 네트워크를 통해 통신할 수 있다.  