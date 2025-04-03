# supabase

터미널에 수파베이스 설치 입력 npm i @supabase/ssr @supabase/supabase-js

루트 디렉토리 생성 utils/supabase/server.ts

.env.local 환경 변수 생성

supabase에서 project setting / data API 가져옴

app 루트 page와 server에 수파베이스 docs문서의 next.js 복붙

## 3계층 아키텍처 구조&#x20;

클라이언트를 :&#x20;

&#x20;1\. Page요청파트 (명령\[키오스크])&#x20;

2\. MenuService 데이터 가공하는 곳(Service\[요리사])을 분리 : 캡슐 : 클래스로 만듬&#x20;

3. MenuRepository 기능 요청 -fetchAll() -create() -update() -delete() = 업무로직임

데이터베이스 : 레코드 추가, 삭제, 반환 ; 데이터를 다루는 기능 = 업무로직이 아님

## 클린 아키텍처 구조(4계층)

UI와 DB에 독립적임 : 업무를 구현하는 로직이 독립

<details>

<summary>clean Architecture</summary>

![](../../../../.gitbook/assets/image.png)![](<../../../../.gitbook/assets/image (2).png>)

</details>

<figure><img src="../../../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

클라이언트:

1\.

IOC : 제어를 역전한다

제어 : 흐름

일반적인 흐름의 반대로 간다

흐름 :&#x20;

재역전 : 모든 프로그램은 객체지향을 말할 때 객체의 조합으로 프로그램을 만듬

객체를 고용을 함

내가 조립하는 사람이고 조립공장 컨테이너가 있으면

컨테이너안에 많은 부품이 있고,&#x20;

조합할 때 제품과 부품, 상황에 따라 달라짐(상대적), 그래서 종속을 피하게 만듬&#x20;

IOC한다는 건 DI를 한다는 것

부품 조립을 한다는 건 부품이 제품일 수도 있으니까 모두 부품 취급함

DepandancyInjection 외부에서 부품을 주입

\*제품이 부품을 만들다가 부품이 커지거나 고치려면 골치아픔

제어의 역전 실습

Page가 요청하면 Service가 필요하고 직접 만드는게 아니라 Repo가 외부에서 물려짐 Entity?

### Domain 계층

페이지 담당 프로그램 도메인 단위로 하나씩 만든다. api로 만들 목적, 노동자 고용

asdf엔티티를 사용해서 데이터를 뽑아네는 것

### APPlication 계층 Use Case 그릇

업무로직 (Use Case)

asdf엔티티

### Infrastructure/repository



domain안에 있는 repo사본의 주체로써 클래스로 구현되어 있음

### Interface Adepter 계층 Control

asdf부모 인터페이스 :: USEcase가 부르면 인터페이스의 자식인 클래스를 연결해줌

\


api계층이 곧 어댑터 계층이다



(\*\*\*\*\*&#x20;

api / munus (목록요청) &#x20;

&#x20;        /menus/new or create : method : POST (새로등록)

&#x20;        /menus/2

&#x20;        /menus/3 : method : PUT

&#x20;        /menus3 : method : DELETE









