---
layout: single
title: "조건문"
toc: true
toc_sticky: true
toc_label: "페이지 주요 목차"
---

### 01. 사주 보기
![sazoo](/assets/images/sazoo.jpg)
~~~c
#include <stdio.h>

int main(void) {
int year, month, day, res;
  printf("당신의 사주를 봐드립니다.\n연도, 월, 일을 차례대로 입력하세요");
  
  scanf("%d %d %d", &year, &month, &day);
  res = year-month+day; if(res%10 == 0) #산술연산자는 같은 줄에 쓴다.
  printf("당신의 사주는 대박입니다.\n");
  else
  printf("당신의 사주는 그럭저럭입니다.\n");
  return 0;
  }
