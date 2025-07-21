---
description: '함수 : 여러 실행문을 하나의 명령어로 정의'
---

# 함수

{% stepper %}
{% step %}
함수



```
 * 형식
	 * 정의 : function 함수명(가인수) { 실행문; return(반환값); }
	 * 호출 :
		 함수명(실인수);
		 or
		 변수  = 함수명(실인수);
	 #가인수  변수를 할당 받을 기억공간 0~여러 개 변수 가능
```
{% endstep %}

{% step %}
함수의 Early return pattern



```
* 정의 : 조건문을 통해 하위에 있는 코드를 실행하지 않고 return 함
	 = 특정 조건에 부합하면 모든 코드 실행안하고 바로 반환
```
{% endstep %}
{% endstepper %}
