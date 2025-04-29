---
description: Additional Description of the Change in Fe and the Need for Next.js
---

# CSR



{% tabs %}
{% tab title="Next.js의 필요성" %}
기업형 프로젝트 ⇒ 규모커짐 ⇒ 업무로직에 따른 컴포넌트 분할 =  Next.js사용
{% endtab %}

{% tab title="Next.js" %}
작용 : 풀스텍 프레임 워크

필요성 : 기존 Fat Client를 완화 하기 위해 컴포넌트까지 서버가 만들어서 전달
{% endtab %}
{% endtabs %}



{% hint style="info" %}
업무로직 : 사용자가 요구하는 로직 = 컨퍼넌트 분할

i 사용자 상호작용 | 키오스크

ii 업무처리 | 요리사

iii 데이터 처리 | 농부
{% endhint %}

{% hint style="info" %}
서버사이드 메인 VS 클라이언트 사이드 메인

⇒  클라이언트 사이드 메인

클라이언트사이드 : 로그인 처리

서버사이드 : 검색엔진 처리
{% endhint %}

***



## FE의 변화와 Terms(Background)

{% stepper %}
{% step %}
**Static Web Page**

client -— server static\[ Only HTML + Added CSS(우선순위로 덮어쓰기)  ]&#x20;
{% endstep %}

{% step %}
**Dynamic Server Web Page**

client --— server\[static + **DB  연동**] 실시간 처리(요구사항)  ex)커뮤니티, 채팅

D-1 : DB 웹서버 환경을 물려서 사용LAMP, WISA스택
{% endstep %}

{% step %}
**Fat Client**

client\[Added **DOM** = JS] --— server\[Dynamic]

D-2 :  클라이언트에 기능 부여(UI 삭제, 변화 기능 등등 ), 서버 연동 사용&#x20;
{% endstep %}

{% step %}
**SPA(Single Page Application)**

client\[Fat Client + JS(XHR)] --— server\[Dynamic]

SPA(Single Page App) : 삭제 말고 추가하는 기능 클라이언트에 추가

&#x20;JS --v up : 덮어쓰기 없이 페이지 하나로 UI계속 바꿈 ex) React

cons : 검색 엔진에 탐색 불가 ; 초기 랜더링 페이지는 키워드나핵심정보를 담지 않음
{% endstep %}

{% step %}
### Full-stack

Frontend(CSR) + Backend(API)

client\[(Angular,  Vue)MVC, (React)flux] --— server\[Dynamic]
{% endstep %}

{% step %}
### Frontend CSR : SSR

CSR : 서버에서 번들을 주면 클라이언트 사이드에서 컨포넌트 렌더링이 일어남

클라이언트가 데이터를 요청하긴함(그러면 API작동)

SSR : 서버에서 렌더링이 일어나서 컴포넌트 번들이 클라이언트로 도착


{% endstep %}
{% endstepper %}



{% hint style="info" %}
DOM : 웹에서   객체화를 진행, JS에서도 html형식을 쓸 수 있도록 만든 나열적 형식

MVC  : DOM객체를 model(변수 + 제어) + view(html) 로 구분화(코드 구조)

flux(코드 구조) : React
{% endhint %}



\
