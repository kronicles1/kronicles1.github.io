---
layout: single
title: "[Coding Test] 자료구조 - 스택/큐"
categories: [codingtest, c++]
sidebar:
    nav: "docs"
---

## 스택
> 스택은 삽입과 삭제 연산이 후입선출(LIFO)로 이뤄지는 자료구조. <br/>
> 스택의 특징 1) 깊이 탐색(DFS), 백트래킹 종류의 문제에 효과적. <br/>
> 스택의 특징 2) 스택의 후입선출 개념은 재귀함수 알고리즘과 원리가 일맥상통. <br/>
> 스택의 특징 3) 스택의 맨 위를 가리키는 용어는 top으로 여기서만 데이터 삽입/삭제가 일어남. <br/>

<br/>

> *스택 선언* <br/>
> #include<*stack*> <br/>
> stack<*int*> myStack; - myStack 변수명의 int형 스택 선언 <br/>
<br/>

> *스택 값 접근* <br/>
> myStack.push(1); - 스택의 top 위치에 1삽입  <br/>
> myStack.pop(); - 스택의 top 위치에 삭제  <br/>
> myStack.top(); - 스택의 top 위치에 있는 데이터 확인  <br/>
<br/>


## 큐
> 큐는 삽입과 삭제 연산이 선입선출(FIFO)로 이뤄지는 자료구조. <br/>
> 큐의 특징 1) 너비 우선 탐색(BFS) 종류의 문제에 효과적. <br/>
> 큐의 특징 2) 삽입/삭제가 양방향에서 이뤄짐. <br/>
> 큐의 특징 3) 큐의 앞을 가리키는 용어는 front, 뒤를 가리키는 용어는 back. <br/>

<br/>

> *큐 선언* <br/>
> #include <*queue*> <br/>
> queue<*int*> myQue; - myQue 변수명의 int형 큐 선언 <br/>
<br/>

> *큐 값 접근* <br/>
> myQue.back(); - back에 있는 데이터 확인 <br/>
> myQue.front(); - front에 있는 데이터 확인  <br/>
> myQue.push(1); - back에서부터 데이터 1 삽입  <br/>
> myQue.pop(); - front에 있는 데이터 삭제  <br/>
<br/>
