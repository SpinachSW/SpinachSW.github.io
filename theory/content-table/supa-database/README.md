---
description: supabase에 (데이터 모델링과 정규화 그리고 제약조건)
icon: '5'
---

# supa-DataBase 구축



* 미래 지향적  : firebase < superbase
* 배포, DB, backend (로직)을 하나 또는 여러 서버에 작업가능
*

{% stepper %}
{% step %}
### Concept Design

저장할 사용자 데이터를 ERD로 선별과정
{% endstep %}

{% step %}
### Logical Design

ERD에서 테이블의 종속, 키, 식별자 관계 분석\[R-DB생성] & 정규화
{% endstep %}

{% step %}
### **Physical Design**

특정 DBMS의 테이블 형태로 사상시키는 과정&#x20;
{% endstep %}
{% endstepper %}

{% tabs %}
{% tab title="업무 시스템(상위)" %}
유기적으로 역할자들이 결합된 집합체

ex) 소모품 담당자, 구매자, 배급자
{% endtab %}

{% tab title="관리 시스템(하위)" %}
문서 관리; 담당 역할자
{% endtab %}
{% endtabs %}
