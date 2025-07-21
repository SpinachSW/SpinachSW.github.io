# API sample

서버 리소스의 위치를 클라이언트 사이에게 전달하는 방식

## Rest Url\[디렉토리 주소]

### 기능

<details>

<summary>api request fcn</summary>

api / munus (목록요청)

&#x20;        /menus/new or create : method : POST (새로등록)

&#x20;        /menus/2

&#x20;        /menus/3 : method : PUT

&#x20;        /menus3 : method : DELETE

</details>

<details>

<summary>예시</summary>

app

&#x20;        /menus

&#x20;        /menus/ new or create

&#x20;        /menus/ 3

&#x20;        /menus/3/edit

&#x20;        /menus/3/delete

</details>

### 페이지 마다 다른 컨포넌트 접근 기능 제공

<details>

<summary><strong>admin예시</strong></summary>

app

||메뉴 관리 시스템

&#x20;        /menus

&#x20;        /admin/menus/ new or create

&#x20;        /admin/menus/ 3

&#x20;        /admin/menus/3/edit

&#x20;        /admin/menus/3/delete

</details>

### 컨퍼넌트가 들어갈 부분

||메뉴 조회 시스템

&#x20;        /menus

&#x20;        /menus/3 || 좋아요 등록은 여기서 함 || React특성 컨퍼런트 쪼개기 수정부분 가능

||좋아요 시스템

&#x20;        /member/likes

||평가시스템

admin, 회원, 익명비회원 다른 종류 페이지 구현하게 됨

## layout&#x20;

app 하위에 layout.tsx생성 (AI children 형식으로 레이아웃 만들어줘)

<details>

<summary>layout</summary>

![](<../../../.gitbook/assets/image (14).png>)

</details>

## Companents 디렉토리

1. 컴포넌트 루트로 관리

<details>

<summary>file</summary>

![](<../../../.gitbook/assets/image (15).png>)

</details>

## 슬러그





