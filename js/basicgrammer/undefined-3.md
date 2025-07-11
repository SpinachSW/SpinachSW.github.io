# 연산자

{% stepper %}
{% step %}
비교 연산자

```
 * ===
	 자료형까지 일치한지?
 * ==
	 값이 일치한지?
```
{% endstep %}

{% step %}
연결 연산자

```
 * 출력에서 변수와 문자열을 같이 출력
 * ex) console.log("가격 : " + price + "원");
```
{% endstep %}

{% step %}
null 병합 연산자

```
 * null일 때 default값 설정
 * ex) 
let num1;
let num2 = 10;

console.log(num1 ?? 20);
console.log(num2 ?? 20);

변수 이중 이용 가능
let num1;
let num2 = num1 ?? 20;
```


{% endstep %}
{% endstepper %}
