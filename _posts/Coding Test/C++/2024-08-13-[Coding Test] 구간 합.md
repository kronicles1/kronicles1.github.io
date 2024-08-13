---
layout: single
title: "[Coding Test] 구간 합"
categories: [codingtest, c++]
sidebar:
    nav: "docs"
---

## 구간 합
> 구간 합은 합 배열을 이용해 시간 복잡도를 줄이기 위한 알고리즘. <br/>
> 구간 합 알고리즘은 우선 합 배열을 구함. <br/>
> 합 배열 S[i] = A[0]+A[1]+...+A[i]; <br/>
> 합 배열을 통해 기존 배열의 일정 범위의 합을 구하는 시간 복잡도가 O(N)->O(1)으로 감소. <br/>
> 합배열 S를 만드는 공식: S[i] = S[i-1]+A[i]; <br/>
> 구간 합(i에서 j까지)을 구하는 공식: S[j]-S[i-1]; <br/>