---
layout: single
title: "[Coding Test] 자료구조 - 페어(노드)/덱"
categories: [codingtest, c++]
sidebar:
    nav: "docs"
---

## 페어(노드)
> 페어(노드)는 자료구조라기보다는 두 개의 값을 하나로 묶어 객체로 만든 클래스. <br/>
> 페어의 특징 1) 두 개의 서로 다른 타입의 값을 저장 가능. <br/>
> 페어의 특징 2) first와 second라는 두 개의 멤버변수를 가지며 각각 첫번째 값과 두번째 값을 가리킴. <br/>

<br/>

> *페어 선언* <br/>
> pair<*int*, string> myPair; - first에 int형, second에 string형 타입의 변수를 갖는 myPair 변수명의 pair 선언 <br/>
<br/>

> *페어 값 접근* <br/>
> myPair.first, myPair.second - 첫번째와 두번째 값 접근 가능  <br/>
<br/>


## 덱
> 벡터와 비슷하지만 앞과 뒤에서 모두 노드 추가/삭제가 가능한 자료구조. <br/>
> 덱의 특징 1) 동적으로 크기가 조정됨. <br/>
> 덱의 특징 2) 양방향 접근성을 지님. <br/>
> 덱의 특징 3) 앞과 뒤에서 삽입/삭제는 O(1)의 시간복잡도를 지니지만 덱 중간의 요소 삽입/삭제 O(n)으로 비효율적. <br/>

<br/>

> *덱 선언* <br/>
> #include <*deque*>
> deque<*int*> dq; - dq변수명의 덱 선언 <br/>
<br/>

> *요소 삽입/삭제* <br/>
> dq.push_back(1); - 뒤에서부터 1 삽입  <br/>
> dq.push_front(2); - 앞에서부터 2 삽입  <br/>
> dq.pop_back(); - 뒤에서부터 요소 제거  <br/>
> dq.pop_front(); - 앞에서부터 요소 제거  <br/>
<br/>

> *요소 접근* <br/>
> dq.front(); - 맨 앞의 요소 <br/>
> dq.back(); - 맨 뒤의 요소  <br/>
> dq[0]; - 0번째 인덱스  <br/>
<br/>

> *덱 관련 유용한 함수* <br/>
> dq.size(); - 덱 내 요소 개수 확인  <br/>
> dq.empty(); - 덱이 비었는지 확인  <br/>
> dq.clear(); - 덱 초기화  <br/>
<br/>