---
layout: single
title: "[Coding Test] 시간 단축에 유용한 코드"
categories: [codingtest, c++]
sidebar:
    nav: "docs"
---

## ios::sync_with_stdio(false);
> C의 stdio와 C++의 iostream을 동기화 비활성화로 C++ 독립 버퍼 사용으로 수행속도 빨라짐. <br/>

## cin.tie(NULL); cout.tie(NULL);
> 하나로 묶인 cin과 cout을 각각 풀어서 서로 다른 작업 전 출력 버퍼를 지우는 작업을 생략해 수행속도 빨라짐. <br/>

## endl->'\n'으로 사용
> cout에서 endl을 사용하면 자동으로 버퍼를 비우기에 반복문에서 성능 저하 일으킴. <br/>
> 따라서 '\n'을 사용해 출력 최적화 가능. <br/>