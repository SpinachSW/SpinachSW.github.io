---
description: ERD에서 테이블의 종속, 키, 식별자 관계 분석[R-DB생성]
---

# Logical Design-\[R-DB]

## 테이블 논리

<details>

<summary> 기존 ERD의 사용관리 논리 정리[R-DB]</summary>

![](<../../../../../../.gitbook/assets/image (10).png>)

</details>

## 테이블 종속적 관계

* ### 종속 지표

<details>

<summary>종속을 알기 위한 태이블 수량적 관계 R-DB</summary>

![](<../../../../../../.gitbook/assets/image (11).png>)

</details>

{% hint style="info" %}
\[1 : N]

주체1가 여러 주체2를 행위하였다. (주체 1 : 주체 2 = 1 : N)

\[N : N]

위 논리가 양방향 (주체) 성립시

\[1 : 1]

행위의 경우 1 : 1 사례 있음(통합 가능할 수 있음)
{% endhint %}

* ### 종속 표시

<details>

<summary> 종속 테이블</summary>

![](<../../../../../../.gitbook/assets/image (12).png>)

</details>

{% hint style="info" %}
1 : N경우 주체의 아이디를 종속된 테이블 FK로 설정
{% endhint %}

## 키

<details>

<summary>키의 종류</summary>

![](<../../../../../../.gitbook/assets/image (13).png>)

</details>

## 식별자

조건 : 자식 테이블의 속성으로 부모를 특정가능

동작 :&#x20;

1. 부모와 식별자 자식 테이블 사이 릴레이션이 실선으로 표시
2. 부모의 아이디인 FK를 자식 테이블의 PK로 사용 = superPK



