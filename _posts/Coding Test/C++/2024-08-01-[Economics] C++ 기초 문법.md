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

## cin.ignore()
> cin.ignore()를 통해 현재 입력 스트림에서 한 문자를 무시한다. <br/> 
> cin.ignore()에 괄호 안에 수 만큼 문자를 무시하는데 기본 default는 1이다. <br/> 
> 괄호 안에 '문자'를 넣으면 특정 문자도 무시 가능하다. <br/> 

## 문자열 입력 받기
> #include < string > 를 통해 string 변수형 사용 가능. <br/> 
> string 변수명 을 통해 문자열 변수 선언 후 getline(cin, 변수명)으로 문자열을 입력받을 수 있다.(공백 포함해서 읽어들임). <br/> 

## 문자열을 문자열 배열로 변환
> #include < cstring >를 통해 strcpy를 사용 가능. <br/> 
> 변수명.length()를 통해 문자열 길이를 입력 받는다. <br/> 
> char* 변수명 = new char[길이 + 1]로 문자열 길이+1(null도 포함해야함)만큼 동적 배열 생성. <br/> 
> strcpy(배열 변수명, 문자열 변수명.c_str())을 통해 문자열 배열로 변환해준다. <br/> 
> delete[] 동적 배열 변수명 으로 동적할당을 해제한다. <br/> 

## 출력시 소수점 표시
> #include < iomanip >.  <br/> 
> cout << fixed << setprecision(소수점 자리 수)를 통해 소수점 표시를 정할 수 있다.  <br/> 