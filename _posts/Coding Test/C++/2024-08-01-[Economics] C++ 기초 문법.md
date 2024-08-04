---
layout: single
title: "[Coding Test] C++ 기초 문법 정리"
categories: [codingtest, c++]
sidebar:
    nav: "docs"
---

## cout
> 기본 설정은 대개 6자리로 출력된다. <br/>
> precision 설정을 통해 소수점 이하의 개수를 정해야 float와 double의 차이를 알 수 있다. <br/> 

## 동적 배열
> c++에서는 변수의 크기를 이용해 배열을 크기를 동적으로 지정하는 것은 허용되지 않는다. <br/> 
> std::vector의 c++ 표준 동적 배열 클래스를 통해 동적으로 변경 가능하다. <br/> 
> ex) std::vector< int > a(num); <br/> 