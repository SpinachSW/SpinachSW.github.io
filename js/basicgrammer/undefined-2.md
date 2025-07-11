# 자료형과 형 변환

{% stepper %}
{% step %}
자료형

```
 * 원시 타입 자료형
	 특징 : 한 번 대입에 하나의 값을 담음
	 ex) 숫자, BigInt, 문자, boolean, null, undefined, symbol 형
 * 비원시 타입 자료형
	 특징: 한 번 대입에 여러 값을 담음
	 객체, 함수, 배열
```
{% endstep %}

{% step %}
형 변환

```
* 동적 타입 언어 let
	 특징 : 다른 타입의 값을 저장해도 값과 함께 타입이 변경됨
* 묵시적 형 변환
	let num1 = "15";
	let num2 = 5;
	
	console.log(num1 / num2); //3
	작용 : 자료형이 자동으로 변환

* 명시적 형 변환
	let num1 = "15";
	let num2 = 5;
	
	console.log(num1 + num2); //155
	작용 : 의도적으로 자료형을 변환
	
```
{% endstep %}

{% step %}
템플릿 리터럴 출력

```
 특징 : console.log에서 문자열과 변수가 함께 출력됨
 python의 f-string과 유사하다.
 형식 : 백틱을 사용해 문자열 변수 작성
 
let name = "hyobin";
let intro = `제 이름은 ${name}입니다.`; 

console.log(intro); //제 이름은 hyobin 입니다.
```
{% endstep %}
{% endstepper %}

