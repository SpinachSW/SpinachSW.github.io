---
description: '호이스팅 : 선언 보다 호출이 먼저 실행 순위에 있을 때, 임시 선언문을 자동으로 적용'
---

# 호이스팅

{% stepper %}
{% step %}
함수



```
* 함수 호이스팅 : 함수의 정의보다 호출문이 상위에 있어도
	 함수의 정의(선언)가 먼저 실행됨
```
{% endstep %}

{% step %}
변수

{% tabs %}
{% tab title="let변수 호이스팅" %}
```
* let변수 호이스팅 :  선언 이전에 사용 불가하도록 처리됨
	불가 원인 : 호이스팅으로 생성된 선언 정의(let num;)가 자바엔진에 의해 TDZ(사용할수없는 공간)로 이동했기 때문
	 let 선언시 공간할당이 자동으로 이루어지지 않음 => TDZ이동
```
{% endtab %}

{% tab title="var변수 호이스팅" %}
```
* var변수 호이스팅 : undifined = 선언 정의를 자동으로 undefined 할당
```
{% endtab %}
{% endtabs %}
{% endstep %}
{% endstepper %}
