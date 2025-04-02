# Rest API

서버 리소스의 위치를 클라이언트 사이에게 전달하는 방식

## Rest Url

### 상태

&#x20;api / munus (목록요청)

&#x20;        /menus/new or create : method : POST (새로등록)

.         /menus/2

./menus/3 : method : PUT

./menus3 : method : DELETE



asdf설계

app

./menus

./menus/ new or create

./menus/ 3

./menus/3/edit

./menus/3/delete

다른 조건의 클라이언트는 다른 접근 권한 기능 제공

⇒ 디렉토리를 조건 클라이언트마다 다르게 만들어야됨

**admin인경우**

app

||메뉴 관리 시스템

./menus

./admin/menus/ new or create

./admin/menus/ 3

./admin/menus/3/edit

./admin/menus/3/delete

||메뉴 조회 시스템

./menus

./menus/3 || 좋아요 등록은 여기서 함 || React특성 컨퍼런트 쪼개기 수정부분 가능

||좋아요 시스템

./member/likes

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





