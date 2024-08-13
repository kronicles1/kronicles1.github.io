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
> #include < vector >
> c++에서는 변수의 크기를 이용해 배열을 크기를 동적으로 지정하는 것은 허용되지 않는다. <br/> 
> std::vector의 c++ 표준 동적 배열 클래스를 통해 동적으로 변경 가능하다. <br/> 
> ex) std::vector< int > a(num); <br/> 

## 동적 배열 push_back()
> #include < vector > <br/> 
> 동적 배열에 원소를 집어넣는 함수이다. <br/> 
> 배열명.pushback(변수명); <br/> 

## 동적 배열 출력
> for(auto& i:배열명){cout << i<<'\n';}으로 동적 배열 vector를 출력할 수 있다. <br/>

## 배열 함수 인자 전달
> vector를 값으로 전달하면 복사본이 전달되어서 main에는 영향이 없다. <br/>
> 따라서 참조에 의한 전달로 하기 위해 void a(vector< int >& 배열명) 으로 전달해주자. <br/>

## 동적 배열 크기 확인
> #include < vector > <br/> 
> 배열명.size()로 배열 크기 확인 가능하다. <br/> 

## 배열 간 겹치는 원소 찾기
> #include < algorithm > <br/> 
> set_interserction(배열명1.begin(), 배열명1.end(), 배열명2.begin(), 배열명2.end(), back_inserter(겹치는 내용 저장할 배열)); 로 가능하다. <br/> 

## 배열 내 원소 곱하기
> #include < numeric > <br/> 
> 배열 내 원소를 더하는 함수 accumulate에서 multiplies< int >() 옵션을 줘서 곱셈이 가능하다. <br/> 
> accumulate(A.begin(), A.end(), 1, multiplies< int >()). <br/> 

## cin.ignore()
> cin.ignore()를 통해 현재 입력 스트림에서 한 문자를 무시한다. <br/> 
> cin.ignore()에 괄호 안에 수 만큼 문자를 무시하는데 기본 default는 1이다. <br/> 
> 괄호 안에 '문자'를 넣으면 특정 문자도 무시 가능하다. <br/> 

## 문자열 입력 받기
> #include < string > 를 통해 string 변수형 사용 가능. <br/> 
> string 변수명 을 통해 문자열 변수 선언 후 getline(cin, 변수명)으로 문자열을 입력받을 수 있다.(공백 포함해서 읽어들임). <br/> 

## getline() vs cin >> string a
> getline은 한 줄을 공백 포함 모두 읽어들임.
> cin으로 string을 입력받으면 공백 문자전까지 읽어들임.

## 문자열을 문자열 배열로 변환
> #include < cstring >를 통해 strcpy를 사용 가능. <br/> 
> 변수명.length()를 통해 문자열 길이를 입력 받는다. <br/> 
> char* 변수명 = new char[길이 + 1]로 문자열 길이+1(null도 포함해야함)만큼 동적 배열 생성. <br/> 
> strcpy(배열 변수명, 문자열 변수명.c_str())을 통해 문자열 배열로 변환해준다. <br/> 
> delete[] 동적 배열 변수명 으로 동적할당을 해제한다. <br/> 

## 출력시 소수점 표시
> #include < iomanip >.  <br/> 
> cout << fixed << setprecision(소수점 자리 수)를 통해 소수점 표시를 정할 수 있다.  <br/> 

## 큰 수 처리하기
> 큰 수는 int형이나 long long으로 처리하지 못하는 경우가 있다.  <br/> 
> 따라서 그냥 문자열로 받아들여 문자열로 처리하는 경우가 많다.  <br/> 

## 정렬
> #include < algorithm >을 통해 sort() 사용 가능.  <br/> 
> sort(배열 시작 주소, 배열 마지막 주소+1)을 통해 정렬이 가능하다.  <br/> 
> 기본적으로 오름차순 정렬을 실시한다.  <br/> 