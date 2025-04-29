# Next.js, supabase 환경 세팅 in vsc

install option

<figure><img src="../../../../.gitbook/assets/image (2) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

## Next&#x20;

React의 프레임워크, 자유도의 규격화 진행

## home Directory 구성&#x20;

&#x20;app(code동적), public(static)&#x20;

{% hint style="info" %}
home Directory : 서비스를 위해 검색하는 홈페이지 Directory
{% endhint %}

<details>

<summary>환경변수</summary>

| 변수                                                                                                            | 설명                                |
| ------------------------------------------------------------------------------------------------------------- | --------------------------------- |
| [`.env`](https://nextjs.org/docs/app/building-your-application/configuring/environment-variables)             | Environment variables             |
| [`.env.local`](https://nextjs.org/docs/app/building-your-application/configuring/environment-variables)       | Local environment variables       |
| [`.env.production`](https://nextjs.org/docs/app/building-your-application/configuring/environment-variables)  | Production environment variables  |
| [`.env.development`](https://nextjs.org/docs/app/building-your-application/configuring/environment-variables) | Development environment variables |

</details>

{% hint style="info" %}
superbase도 환경변수로 들어감

Git commit할 때 환경변수는 gitignore에 명시할 것; 커밋 제외
{% endhint %}

## 폴더 &링크 관리

{% embed url="http://localhost:3000/" %}

{% embed url="http://localhost:3000/menu" %}

즉, 폴더를 만드는것은 url을 만드는 것&#x20;

<details>

<summary>폴더예시</summary>

![](<../../../../.gitbook/assets/image (1) (1) (1).png>)

</details>

## vscode supabase 불러오기

터미널에 수파베이스 설치 입력 npm i @supabase/ssr @supabase/supabase-js

루트 디렉토리 생성 utils/supabase/server.ts

.env.local 환경 변수 생성

supabase에서 project setting / data API 가져옴

app 루트 page와 server에 수파베이스 docs문서의 next.js 복붙



중간 예시 디렉토리(API, adepter 제외)

next 기본형 + 클린 아키텍처 adepter 제외

<details>

<summary>루트 app</summary>

![](<../../../../.gitbook/assets/image (3).png>)

</details>

<details>

<summary>클린 아키텍처 루트 application / usecases</summary>

![](<../../../../.gitbook/assets/image (4).png>)

</details>

<details>

<summary>domain 클린 아키텍처 repository</summary>

![](<../../../../.gitbook/assets/image (5).png>)

</details>

<details>

<summary>클린 아키텍처 infra repositories</summary>

![](<../../../../.gitbook/assets/image (6).png>)

</details>

<details>

<summary>클린 아키텍처 ? 유틸 수퍼베이스 서버, 그외</summary>

![](<../../../../.gitbook/assets/image (8).png>)

</details>

