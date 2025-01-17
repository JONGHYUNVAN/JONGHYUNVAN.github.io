---
title: 객체지향 프로그래밍
keywords: sample
summary: "This is just a sample topic..."
sidebar: product1_sidebar
permalink: p1_sample1.html
folder: product1
---

## 객체지향 프로그래밍 기초
객체지향 프로그래밍을 배워볼거다.   
학습 목효는   
객체지향 프로그래밍의 가장 기본적인 토대인 객체를 이해.     
객체를 만드는 데 필요한 클래스의 개념과 문법 이해.   
객체의 두 가지 구성 요소, 속성과 기능 이해.   
클래스에 기반하여 new 키워드를 통해 객체 생성.   
클래스와 객체의 차이와 언제 무엇을 사용해야 하는지 이해.   


## 객체가 뭔데 ?

모든 '실재하는 대상'을 프로그래밍 언어에서는 객체(Object)라고 부른다.   
사물과 같은 유형적인 것뿐만 아니라, 개념이나 논리같이 형태가 없는 것들도 다 객체다.   
프로그램 입장에선 '메모리에 있는 것'이 곧 객체가 되겠다.   
참고로 객체지향 프로그래밍의 상대적 개념으로 절차지향 프로그래밍이 있다.
메소드별로 묶지 않고 컴퓨터가 인식하는 순서로 쭉 풀어짜는 식의 프로그래밍인데, 일단 컴퓨터가 명령의 기능이 어디 적혀있는지 찾지 않는다는 점에서 빠르다는 장점이 있다.   

예를들어 '개미 로봇' 의 경우를 생각해보자.   
개미의 머리는 처리해야할 정보가 많다. 물체와의 거리가 어느정도인지,지금 걷기를 멈춰야 하는지, 
턱을 어디까지 낮춰야 하는지, 턱에는 힘을 얼마나 주고 목에는 힘을 얼마나 줘야 들 수 있는지,   
또한 새로운 기능을 추가할 수도 있다. 이럴 때는 각각의 기능을 객체로 묶어야 변수가 꼬일 일도 적고,
필요한 기능에의 접근도 쉬워진다.   
개미의 다리는 상황이 다르다. 다리는 '걷기' '방향전환' 두가지 기능만 한다. 움직이는 다리의 순서가 바뀌면 개미는 의도대로 움직일 수 없으므로,
다리의 동작에서 가장 중요한건 동작 순서이고, '걷기' 에서 '방향전환' 으로 동작을 변경하더라도 현재 다리의 이름이나 다리기 알미나 굽혀있는지
등의 정보가 변하면 안된다.   
따라서 개미의 머리는 객체지향 프로그램, 개미의 다리는 절차지향 프로그래밍이 이상적이다.

## 왜 객체지향 프로그래밍을 배우는데 ?

프로그램 개발 및 유지 보수에 드는 비용과 시간을 획기적으로 줄일 수 있고, 객체를 통해 데이터를 관리하여 데이터를 손실 없이 관리하기에 용이하다.   
같은 코드 복붙하고 복붙하고 할 거 없이 "이것"을 정의하고 "이것" 해라 라고 하면 편한것처럼.