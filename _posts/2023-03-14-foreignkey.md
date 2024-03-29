---
layout: post
read_time: true
show_date: true
title: 외래키란?
date: "2023-03-14 18:23:20"
description: 외래키에 대해서 알아보자
tags:
  - Database
author: ParkWonyeop
published: true
img: ":title.png"
category: database
---

## 서론

데이터베이스 설계는 저장된 데이터의 효율성, 무결성 및 일관성을 보장하는데 중요한 역할을 한다.  
관계형 데이터베이스의 설계의 기본 개념 중 테이블 간의 관계를 설정하고, 데이터 일관성 및 참조 무결성을 보장하는데 사용되는 것이 외래키이다.  
오늘은 외래키의 개념을 알아보자.   

## 외래키란?

외래키는 테이블 간의 기본키를 참조하는 테이블의 컬럼 또는 컬럼의 집합이다.  
외래키의 목적은 관련있는 테이블 간의 관계를 설정하여 데이터베이스가 참조 무결성을 유지하고 테이블 간의 관계를 일관되게 만드는데 있다.  

## 외래키의 중요성

외래키를 설정해야하는 이유는 아래와 같다.  

### 참조 무결성  

외래키는 참조 무결성을 유지하는데 중요한 역할을 한다.  
외래키를 설정해 테이블 간의 관계가 일관되고, 고아객체와 일관성없는 데이터가 생기지않게 방지하는 역할을 한다.  

### 쿼리문 최적화

외래키는 테이블 간의 관계에 대한 힌트를 제공하여 데이터베이스 쿼리를 최적화하는데 도움을 준다.  
이는 보다 효율적이고 빠른 쿼리문 실행에 도움이 될 수 있다.  

## 마치며

외래키는 관계형 데이터베이스 설계의 중요한 개념으로 테이블 간의 관계 설정을 가능하게하고 데이터 일관성 및 참조 무결성을 보장한다.  
외래키의 개념과 그 중요성을 이해하는 것은 데이터 관리 및 데이터베이스 성능을 최적화를 하는데 용이할 것 이다.  

