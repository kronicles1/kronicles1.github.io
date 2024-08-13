---
layout: single
title: "[Coding Test] 형변환"
categories: [codingtest, c++]
sidebar:
    nav: "docs"
---

## string -> 숫자형
> #include < string > - 헤더파일 필요 <br/>
> string sNum; <br/>
> int inum = stoi(sNum); <br/>
> long lnum = stol(sNum); <br/>
> double dnum = stod(sNum); <br/>
> float fnum = stof(sNum); <br/>

## 숫자형 -> string
> #include < string > - 헤더파일 필요 <br/>
> int inum = 1234; <br/>
> string sString = to_string(inum); <br/>
> 다른 숫자형에 대해서도 동일하게 to_string 사용 가능 <br/>