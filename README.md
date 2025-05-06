# TIL
## HTML태그
* block : h, p, blockquote, address, hr, div, a(i), video
* inline : br, strong, em, s, del, sub,sup, q, code, span, 
## Vs code 단축키
* `ctrl + k` -> `ctrl + \` 위/아래 수직 화면 분할
* `ctrl +\` 좌/우 수평 화면 분할
* `ctrl + j` 터미널 실행 / 닫기
* `Q` or `ctrl +c` 터미널 입력안되는 에러 해결 단축키
## 작업폴더 설명
* `html_basic/` : html 기초 연습파일
* `task/` : 과제제출 폴더, 파일 모음(폴더명은 날짜별로 구성)
* `README.md/` : 배운 내용 기록, 어려운 점 및 막힌 점 자유롭게 기록
----
### 2025/04/04 <HTML 3일차 - 문서와 레이아웃>
* `h1~h6`, `p`, `br`, `storng`, `em`, `del`, `s`, `sup`, `sub`
* TIL 자유롭게 작성 -> 공부기록, 프로젝트기록, 과정 등등 세세하게 기록. 블로그 기록하듯이 
----
### 2025/04/07 <HTML 4일차 레이아웃>
* `div`,`span`
* 웹/앱 레리아웃 방향과 의미에 따라 2개 이상의 요소를 묶어주는 레이아웃 요소
* `div`는 생성 시 반드시 그룹을 구분할 수 있는 이름을 설정해야 한다.
* `span`은 선택!

### 태그+이름속성 Class, id
* .Class: 반복 유형 분류 시 사용, 반복지정가능
* #id : 전체 페이지 중 단 하나의 요소에만 지정 시 사용 -> header, footer
* Class, id는 태그 관계없이 모든 태그에 적용 할 수 있다.
* .,# 은 css언어이기때문에 html에서는 사용하지 않음.

* 이름작성시 주의사항 : 반드시 용도에 맞는 의미있는 영단어 사용!
* 다른 단어는 구분해서 작성 -> title_g
* 길게 쓰더라도 의미있게 작성하는게 중요

### HTML 구조
1. 클론 코딩 & 클론 디자인할 사이트 정하기
2. 피그마에서 와이어프레임 만들기 (레이어, 폴더 이름주의)
3. 피그잼에 일부 화면 넘겨서 태그 게획하기
4. 계획한 태그를 가족관계에 맞게 트리구조 만들기
5. Vs code에서 실제 HTML 작성하기 (트리구조 순서에 맞게 바깥쪽 -> 안쪽 순서로!)

### 다른 환경에서 git 이어서 작업하기(집)
* 새폴더 연결하기
* `git clone 저장소 주소 붙여넣기`
* `CD 저장소 폴더명`적고 수정하고 파일 저장
* `git status` 상태 확인
* `git add .` 파일 스테이징 업로드
* `git status`로 업로드 확인
* `git commit -m '메세지'`작성
* `git push origin main` github 업로드
### (위 이어서)다른 환경에서 git 이어서 작업하기(학원)
* `git pull origin main` 집에서 올린 파일 내려받기

### 바로가기 메뉴 만들기
0. (조건) 화면이 수직으로 충분히 이동할 수 있을만큼 세로 스크롤 준비
1. 바로가기 메뉴 a 태그 준비하기
2. 바로가기 위치 < div id > 이름 준비하기
3. 위 1번 `a` 속성 `href` 값으로 `#`먼저 작성 후 위 2번 이름 작성해서  a 태그 완성하기
4. 위 3번 결과 예시) id가 abcd일 경우 `<a href="#abcd"></a>`
-----
### 2025/04/08 <HTML5일차 - >
----
### 2025/04/09 <HTML 6일차차>
## a 태그가 그룹일 때 href="#" class="" 잊지말고 작성하기
## 이미지태그 `<img>`
### (i) `<img>` 태그
* src 이미지 경로 속성의 값으로는 상대경로 방식으로 작성 권장
* 이미지 사용 시 의미 전달이 필요한 이미지와 아닌 이미지를 구분해서 사용
* 필수
* `<img src=”url”>`
## 이미지 태그 필수속성  `<img alt>`
* 대체텍스트 alt 속성을 필수로 작성 → 키보드 alt랑 다름
* 필수
* `<img src=”url” alt=””>`
* ex) `<img src=”url” alt=”접근성 오픈 아카데미 유튜브채널 구독하기. 매주 월요일 콘텐츠 업데이트합니다.”>`
----
### 링크 복습
* `<a href="#">< /a>` 임시링크 (다음 페이지 제작 전일 경우)
* `<a href="#header">< /a>` 바로가기 링크, id header로 이동한다. (같은 파일 내 다른 위치 이동)
* `<a href="./basic/index.html"></a>` 상대경로링크, 현재위치에서  basic 폴더 안에 html파일로 이동한다.
* `<a href="./basic/index.html#main></a>` 상대경로링크+바로가기링크, 현재위치에서 basic 폴더로 들어가서 index.html 안에 main 위치로(특정위치) 이동한다.
----
### 2025/04/10 <HTML 7일차 - 정의형 목록태그와 메뉴개념념>
* `html:5 tap` html 자동완성 작성
   -> 자동완성은 head와 body가 들여쓰기 X
* `<meta name="viewport" content="width=device-width, initial-scale=1.0">`
   : 사용자가 보는 화면의 너비가 디바이스의 너비의 1.0비율로 맞춰지게 하겠다
## 정의형 목록태그
### 정의형 목록 기본 작성법
* 정의형 목록은 dl,dt,dd 3가지 태그로 이루어져 있다
* dl은 정의형 제목과 내용을 묶는 그룹 -> class 속성을 가진다
* dt는 dl 안 자식으로 배치, 제목을 의미
* dt는 dd 기준 항상 먼저 시작
* dd는 dl 안 자식으로 배치되며 dt의 다음 형제 요소로 배치되거나 기존 dd의 형제로도 배치될 수 있다
* 레벨이 없이 사용, 보통 2~3, 대제목 자리에는 사용 불가
* p 여러개 자리에 dt-dd-dd로 대체 가능
* h 처럼 제목이 독립적이지 않아서 dt, dd는 항상 같이 작성 (dt dt dd X)
### 내비게이션 메뉴 태그
* gnb(global navigation bar)
: 사이트 최상단 내비게이션 , 어떤 페이지에 들어가도 고정되어있는 주 메뉴
* lnb(local navigation bar)
: gnb의 하단에 배치된 서브 메뉴, 중분류 메뉴 -> gnb 하위메뉴
* snb(side navigation bar)
: 페이지 내에 좌/우측에 일반적으로 존재하는 추가 메뉴, 서브메뉴X -> 사이드메뉴
* fnb(footer navigation bar)
: 사이트 최하단 내비게이션, footer영역에 존재하는 회사소개, 저작권 등의 보조메뉴 
* BreadCrumbs(브레드크럼)
: 서브페이지에 표시된 현재 페이지 경로(헨젤과 그레텔의 집을 찾아가기 위해 길에 빵부스러기를 버린 예시)
----
### 2025/04/11 <피그마 - 프로토타입>
### 스타일가이드 만들기
----
### 2025/04/14 <css day-1>
## css 파일은 반드시 styles 폴더 안에 만들기
## css (cascading style sheets)
: 사용자에게 시각적으로 보이는 문서를 꾸미는 언어
* 폭포 단계별로 적용하여 디자인하는 css 언어구성
* 위에서부터 단계별로 디자인 진행
## 선택자{속성:값;}
* 선택자 : css로 디자인하는 대상 -> 태그, class, id
* {} : 속성과 값을 묶어주는 css 디자인 괄호
* 속성 : 선택자에 적용하는 속성
* 값 : 속성값
* ; : 속성값이 여기서 종료했다는 것을 의미
## 속성
* color 글자색
* background-color 배경색
## css 작성방법
1. 내부스타일 <head> 태그내에 <style> 태그로 작성
2. 외부스타일  별도의 css 파일을 작성하여 <link>태그로 연결
* html 내부에 작성하는 css는 해당 html파일에만 종속되서 외부 html에 연결할 수 없다. 이런 비효율적인 문제때문에 실제로는 외부스타일이 많이 사용된다. 
### 부모-자식,자손 선택자
### 형제 선택자
----
### 2025/04/15 <css day-2>
## 글자표현속성
### font-family
* 대표글꼴, 후보글꼴1, 후보글꼴2
* 대표 글꼴이 무넺 발생 시 대체해서 나갈 수 있도록 후보글꼴이 대기
* 특징이 비슷한 것들로 연결
* 글꼴명이 한글 또는 공백이 포함되어 있을 경우 따옴표로 묶어서 작성
### font-weight
* 글꼴 굵기 설정값, 400(기본값) 100단위로 크고작아지면서 조절
### font-size
* desktop 환경의 글자크기 : 16px
* mpbile / tablet 환경의 글자크기 :14px
* px 단위는 절대 크기값이라 사용자별 글자크기를 지원하지 않기 때문에 상대적 단위인 em, rem, %를 사용한다. 그중에서도 `rem`을 많이 사용한다.
* `rem`은 부모의 값과 상관없이 나만의 크기를 인식하기 때문 
### line-height
* line-height:1.5;
* 행간은 디자인 상황에 따라 px과 %를 적절히 사용
* `피그마 170% -> css :1.7;`
* line-height를 이용한 수직정렬
   * line-height을 이용한 수직정렬 주의사항
   ->요소의 height값이 px로 작성된 경우(조건) 그 값을 그대로 line-height의 px값으로 작성하여 수직 가운데 정렬을 적용한다. 단, 글자가 2줄 이상일 경우 사용해서는 안되며 (주의)1줄일때만 사용해야 한다.
### text-align 수평정렬
* text-align 속성은 속성값을 입력한 대상 기준으로 그 자식 또는 자손이 `인라인` 요소일 경우만 적용된다. 
* 단순 글자도 인라인으로 인식함.
* block은 적용 X
### letter-spacing / word-spacing
* letter-spacing:-0.02em;
* `figma -2% -> css -0.02em`
### width:; height:; 가로세로
### text-align:;
### margin-top:;
### margin-bottom:;
### display:inline-block;
### border-radius 모서리 둥글기
### 블록을 가운데 정렬하는 방법
`margin-left:auto;`
`margin-right:auto;`
* 반응형 -> 보는 사람마다 자동으로 여백을 처리해서 가운데로 정렬(규칙)
* text-align은 인라인만 적용되기 때문에 이 방법으로 블록 가운데 정렬
----
### a태그 선택속성 title
* a태그에 마우스를 올리면 나오는 말풍선같은거
----
## 정리
## CSS style sheet
* 외부스타일시트 파일 저장 **styles**폴더에 `파일명.css`저장한다.
* 위 파일 생성 후 css연결을 원하는 html파일 head 위치에 `<link>`태그로 연결한다.
* html 작성 후 html의 모든 디자인 형태를 초기화하는 `reset.css` 반드시 연결.
* 웹글꼴(noto sans kr,pretendard 등) 연결 시 html파일에 `<link>`태그연결
### head태그 내에 들어가는 link태그 작성순서
1. 웹글꼴 포함 기타 플러그인 연결 주소
2. reset.css
3. 해당 html별 디자인 css 파일
### 디자인 css작성 시 작성 순서 및 주의사항
* **부모->자식**순서로 가장 바깥쪽 부모부터 먼저 선택자를 만들고 디자인한다.
* 레이아웃 관련 요소에 `width, hright` 속성 작성 시 영역 확인을 위한 `background-color`를 꼭 함께 작성해서 정확히 구분한다. 이 때 색상은 쉬운 영역 구분을 위한 `aqua, lime, yellow, pink`등의 밝은 색상 위주로 사용한다. 영역 확인과 디자인 작업을 모두 마친 후 위 색상은 제거로 마무리한다.
* 실제 디자인에 들어가는 색상은 **rgba 또는 헥사코드**로 입력하고 테스트용 색상은 영문명으로 입력한다.
### 자주 이용하는 css 속성 값과 기본값
* `letter-spacing` 자간 | 0 | `letter-spacing:-0.02rem;`
* `line-height` 행간 | 1 (100%) | `line-height:1.5;`
* `font-size` 글자 크기 | 16px (1em) | `font-size:1.25rem;`
* `color` 글자색상 | `color:#111; color:rgba(0,0,0,0.5);`
* `background-color` 배경색상 | `background-color:#000;`
* `width` 가로 크기 | `width:200px`;
* `height`세로 크기 | `height:200px;`
* `margin` 바깥쪽 여백 | `margin-top:50px;`
* `border-radius` 모서리 둥글기 | `border:50px;`
* `font-weight` 글자 굵기 | 400 | `font-wieight:500;`
* `font-family` 글자 설정 | `font-family:대표글꼴, 보조글꼴, san-serif;`
----
### 2025/04/16 <css day-3>
## html5 시멘틱태그
* 의미있는 태그의 모음
1. `<header></header>`
* 로고 및 내비게이션을 묶어주는 웹 가이트 레이아웃 태그
* 제목, 로고, 검색 폼, 작성자 이름 등의 요소도 포함
2. `<nav></nav>`
* 로고 및 웹사이트 주요 내비게이션(gnb)을 묶어주는 웹사이트 레이아웃 태그
* 다른 페이지로서의 링크를 보여주는 구획.
* 주로 메뉴, 목차, 색인에 쓰인다.
* gnb를 묶는 태그 ul (nav의 자식 ul)
* footer에는 사용 x
3. `<section></section>`
* 문서의 독립적인 구획을 나타내며 제목을 포함하는 경우가 많다.
* section 밑에 자식으로 h (필수는 아니지만 경고가 생김)
* 여러개일 경우 class 이름주기
4. `<aside></aside>`
* 문서의 주요 내용과 간접적으로만 연관된 부분
* 주로 사이드바 혹은 콜아웃 박스로 표현
* 비교적으로 좁은 부분은 aside일 가능성이 높다.
5. `<article></article>`
* 사이트 안에서 독립적으로 구분해 배포하거나 재사용할 수 있는 구획
* 공유 가능한 게시판과 블로그 글, 메거진이나 뉴스 기사 등등
6. `<footer></footer>`
* 웹페이지 가장 하단에 위치
* 구획의 작성자, 저작권 정보, 관련 문서 등의 내용을 담는다.
7. `<main></main>`
* 문서 <body>의 주요 컨텐츠 (header 밑에서부터 footer 전까지)
* 주요 콘텐츠 영역은 문서의 핵심 주제나 앱의 핵심 기능에 직접적으로 연결됐거나 확장하는 콘텐츠로 이루어짐
## 입력 및 선택 컨트롤 양식
### (b) form 폼
* 사용자로부터 입력 받을 수 있는 폼을 정의하는 요소
* 입력하거나 선택하는 것을 묶어주는 틀
* 사람마다 선택하는 것이 다 다르게 컨트롤 할 수 있다면 폼 (선택했을 때 다 같은 행동은 한다 -> link)
* action : 폼 데이터를 제출할 서버 스크립트 지정 -> 서버에서 확인하는 작업
* method : 폼 데이터를 제출하는 방법
 * POST : 폼 데이터를 HTTP 본문에 포함하여 서버로 전송.(보안높음) -> 로그인, 회원가입, 설문조사, 보안이 중요한 정보
 * GET : 폼 데이터를 URL에 추가하여 서버로 전송.(보안낮음) -> 검색결과, 보안이 중요하지 않은 정보
### (b) fieldset
* 양식의 일부를 그룹화하는 태그. legned 그룹 제목 포함
* 폼의 양식을 더 읽기 쉽고 이해하디 편하게 구성하는데 주 목적
* (i) legend -> fieldset에는  class or id를 쓰지 않고 legend를 작성
* 디자인에서는 숨김처리 하기 때문에 `reset.css` 파일에 작성한다
* 숨겨지는 태그이기 때문에 블록과 형제로 써도 상관 X
### (i) input type="" 입력 필드 속성
* `input type="text"`
* `input type="password"`-> 보안
* `input type="number"`
* `input type="email"`
* `input type="search"`
* `input type="date"`
* `input type="time"`
* `input type="url"`
* type = input 요소가 나타낼 입력 필드의 종류를 정함
* name = input 요소의 이름을 지정 (데이터 구분)
* value = ibput 요소의 초기값을 지정 -> 필수X  ex) 쇼핑몰 수량 1
### input 속성
* maxlenght : 크기 size와 글자 수 제한 설정 
* required : 필수 입력 필드 지정
* readonly : 읽기전용 -> 선택 X, 컨트롤에 따라 변경되는 것 
* disabled : 필드 비활성화
* `<input type="text" size="" manlenght="">`
* `<input type="text" required>` -> 속성과 값이 동일할 경우 하나만 작성 (video태그에서 autoplay, mute...)
* `<input type="text" readonly>`
* `<input type="text" disabled>`
* autocomplete : 자동완성기능 -> 검색, 아이디, 이메일...
* accrpt : 요소에서 허용하는 파일 형식 지정
* multiple : 입력 필드에 여러 이름 입력 시 각 개별 값 처리
* `<input type="text" autocomplete="on">` -> on, off, new-password, email, trl, url
* `<input type="text" accept="image/png">` -> application/pdf , * (* : 모든파일)
* `<input type="text" multiple>`
* `<input type="file">` -> 파일 선택
### textarea 여러줄의 텍스트를 입력할 수 있는 입력필드
* name = 요소 이름 지정
* value = 요소 초기값 지정
* rows = 요소의 세로 크기
* cols = 요소의 가로 크기
* disabled = 요소 비활성화
* placeholder = 요소 입력 텍스트 지정 -> 입력 안했으르 때 보이는 안내문
* required = 필수 입력 처리
* form = 요소가 속한 폼 지정
### (i) input type=”” 선택 필드 속성
* input type=”radio” 하나만 선택
* input type=”checkbox” 두개 이상 선택
* select
* type = 요소가 나타낼 타입 지정
* name = 요소의 이름 (같은 선택에 포함 될 경우 동일한 이름 처리) → 동일한 이름으로 처리하는 그룹
* value = 요소의 가진 고유의 초기값 지정→ 고유 정보로 데이터를 구분하는 전송값, 선택 양식을 구분하는 데이터값
* ex) 남 `<input type="radio" name="gender" value="male">`
* ex) 여 `<input type="radio" name="gender" value="female">`
### (i) Label
* input 입력,선택 필드의 접근성을 높이는 Label for=”” 
* `<label for=”target”></label>`
* `<input type=”radio” name=”” value=”” id=”target>` → id랑만 연결, 단 하나의 요소, value랑 같은 이름 사용가능
### (i) button
* **`<button type=”button”>기본</button>` 범용기능, 전송 취소 웹앱의 버튼 기능… 모두**
* **`<button type=”submit”>제출</button>` 전송 action 으로, 서버로 전송**
* **`<button type=”reset”>초기화</button>` 삭제,취소,초기화**
* → 대부분 button으로 만들고 자바스크립트로 동적 처리
**주의**
### button과 a
* a → 선택했을 때 한 가지 링크로 연결, 다 같이 한곳으로 이동
* button → 선택했을 때 분기가 나누어짐, 사용자에 다라 다른 동작을 수행
----
### 2025/04/17 <css day-4 / html>
### 블록의 너비값을 부모보다 적게 설정했을 때 블록을 가운데 정렬하고 싶다면?
`margin-left:auto;`
`margin-right:auto;`
### font -> (r)em
* 12px = 0.75rem
* 13px = 0.813rem
* 14px = 0.875rem
* 15px = 0.938rem
* 16px = 1rem
* 18px = 1.125rem
-----
### 25/05/18 <css day-5>
## 요소표시속성 display
* 블록 또는 인라인으로 표시 속성을 변경하여 외부 표시 유형을 설정
* `display :block;`
* `display :inline;`
* `display :inline-block;`
* 요소 숨기기/보이기 : `display :none or block`(요소에 따라)
* 레이아웃 변동 없이 요소 숨기기/보이기 : `visibility :hidden or visible`
## 요소의 크기 속성 width/height
* px , % , vw/hw
* width :100px → 절대값, 부모영향X
* width :100% → 부모 기준까지
* width :100vw → 보이는 화면 영역에 맞추기 / 화면을 켜면 바로 사용자에게 보이는 크기
* 너비로 작성했지만 h 높이도 동일한 의미
## padding, margin (안쪽 여백, 바깥쪽 여백)
* padding 요소의 안쪽을 벌릴 때(부모-자식)
* margin 다른 요소(형제)와 요소 사이에 거리를 벌릴 때
#### 여백 읽는 순서
* 시계 방향 top → right → bottom → left
 * margin : 20px 30px 40px 50px; (값이 0이 아닐 때는 px붙이기)
* 모든값이 동일 →  padding:50px;
* padding:50px;   상하좌우의 모든 값이 동일할 때 값 1개 
* padding: 1px 2px 3px 4px;   위,오른,아래,왼 값이 각각 다를 때 
* padding:5px 10px;   상하.좌우 값이 2개씩 같은 경우 앞:상하 뒤:좌우 
* padding:5px 10px 0;   상.좌우.하 값 3개 나누기 -> 좌우는 같고 상하가 다를 때 
## border 테두리 속성 
*  border:두께 모양 색상;
* ex) border:1px solid red;
* ex) border:1px dashed black;
* ex) border:1px dotted coral;
* ex) border-radius:10px; (%)
## 표태그 table
### (b) table
* 테이블 관련 태그는 모두 block
* 테이블의 기본 테두리 값은 0으로 css를 진행하기 전 1px 설정을 권장
### (b) tr행, td내용 열
* 열(td)는 항상 행(tr) 안에 존재
* 테이블은 행, 열을 자식, 자손으로 가지는 부모로써 존재
* 블록이지만 크기를 안주면 내용만큼만 크기를 갖는다
### (b) th 제목 열
* (b) thead, tbody, tfoot 행 그룹
 * 행그룹은 행(tr)의 부모로 사용
 * thead : 제목행그룹, th위주로 구성된 제목행(tr)을 묶을 때 사용
 * tbody : 내용행그룹, td위주로 구성된 내용행(td)을 묶을 때 사용
 * tfoot : 결과행그룹, th&td들로 구성된 결과값을 가지는 결과행(tr)을 묶을 때 사용
* 속성
 * colspan (수평열 합치기) / rowspan (수직열 합치기)
1. 합치고 싶은 가로방향 열 2개 이상 정하기(개수제한없음)
2. 위에서 정한 태그 확인하기
3. 위 태그 중 먼저 시작한 태그속성으로 colspan:"합치는 칸의 개수"
4. 합쳐지는 첫번째를 제외하고 나머지 태그는 주석으로 가리기 
-----
### 25/04/21 <css day-6>
## 수열선택자
#### :nth-child(n)
* css에서 요소를 규칙적으로 선택하고자 할 때 사용하는 선택자
* :nth_child(n) 형태로 작성되며, 반복패턴을 따라 자식이 2개 이상 있을 때 n번째 자식이란 개념으로 선택한다. 클래스와 아이디로 의미있는 이름을 짓기 적합한 대상이 아닌 경우 이름을 짓지 않고 css 선택이 가능해 다양한 경우에 유용하게 사용
* ex) li:nth-child(2) {background-color:red;} → 목록 중 2번째 자식 li를 선택해서 배경색을 빨강으로 한다.
* 첫째와 막내는 first-child / last-child 로 작성 가능
#### :nth-of-type(n)
* th-child(n) : 전체 형제 요소 중 n번째 대상
* nth-of-type(n) : 전체 형제 기준 태그 종류 중 n번째 대상
#### :nth-child(An)
* A : 반복간격(주기)
* :nth-child(3n) 3간격으로 형제 요소 선택하기(3의배수)
 * 3,6,9,12,15,18,21….번째 요소 선택
 * 목록(li)에서 많이 사용
 #### :nth-child(An+B)
 * A : 반복 간격 (주기)
 * B : 시작위치
 * :nth-child(3n+1) 1번부터 시작해서 3의배수(3개 간격으로)
 * 1 4 7 10 13 16….
#### :nth-child(odd) 홀수
#### :nth-child(even) 짝수
## 배경속성
### background-color
### background-image:url(경로);
* 상대경로 작성기준 (주로 상대경로로 작성함)
* X,Y 무한반복(기본값) → 이미지 크기에 따라 반복되는게 달라짐
* 선택자에 색상을 넣은 상태에서 이미지는 색상 위로 배치된다.
* 같은 이미지를 사용하려면 공통 선택자에 작성
* 글자나 주변 다른 요소들과 겹쳐지고 밑으로 이미지가 보인다면 background-image
* 단독으로 사용되면 <img> 태그
* 절대경로로
### background-repeat:반복설정;
* repeat (기본값)
* no-repeat : 반복안함
* repeat-x : 옆으로만
* repeat-y : 밑으로만
### background-position:방향
* x,y,순으로 작성
* left top 기준
* ex) 100px 20%
### background-size
* contain : 요소 안에 배경 이미지가 전부 나타나도록 가로 세로 크기를 조정. (가로세로는 이미지의 형태에 따라 빈 부분이 생길 수 있다. → 이미지를 자르지 않고 다 보여줌)
* cover : 배경 이미지로 요소의 크기를 모두 덮어 씌우는 형태로 적용. (빈 부분 없이 이미지로 꽉 채움 → 이미지가 잘릴 수 있다.)
* :300px auto; : x,y 값 순서로 %,px,auto단위 값을 적용 (auto = 자동비율) → 비율 지키기
### background-attachment
* background-attachment:fixed or scroll(기본값);
* 화면 스크롤과 함께 배경 이미지가 움직인다면 = scroll(기본값)
* 화면 스크롤 상관 없이 배경 이미지가 고정된다면 = fixed
* **image - repeat -position - size - attachment : 이미지 관련 속성. 같이 연관 지어서 같이 알고 있어야 함**
### background 통합 속성 버전
* **background: color image repeat attachment position / size**
*  순서만 지켜서 사용하고 싶은 속성만 작성 가능
* 부모에 속성을 적어도 통합 속성에서 적지 않으면 css 기본값으로 인식
* 공통 css를 적용하지 않을 경우 통합 속성으로 필요한 속성만 작성
* size는 마지막에 / 쓰고 작성하기

-----
### 25/04/24
## 위치속성 float
* 블록, 인라인 요소를 좌(left), 우(right) 사용하는 위치 속성
* 배치하는 좌우 요소가 **형제**인 경우 사용
* 형제가 3개 이상인 경우 1 ->2 옆으로 두고 3을 내리고 싶은 경우, 형제 3에게 `clear:both`를 선언하여 이전 형제의 float 정렬 제거하기
### 오른쪽으로 보내고 싶은 형제 요소가 2개 이상이라면?
* 2개를 묶어서 그룹으로 처리하고 `float:right` 한번만 작성한다.
* `float:right`는 2번 이상 사용하면 역순이 되므로 **한번만 작성한다!!**
### float를 적용하는 형제의 부모의 높이가 max-content(기본값)이라면?
* 부모의 높이를 제대로 인식못하므로 높이를 강제(px)시키거나 `overflow:hidden`으로 높이를 안주고 영역 재인식을 시켜 float에 의한 오류를 제거해야 한다.
## 상대선택자
### hover
* 사용자가 마우스를 올렸을 때 상태에 따라 스타일을 적용
* a {color:blue;}
* a:hover {color:red;} → 블루로 보이다가 마우스를 올리면 빨강으로 바뀐다.
* button {background-color:orange;}
* button:hover {background-color:red;}
* 선택자를 복사해서 새로만들어서 예를 들어 그림자 디자인을 넣었는데 위아래 그림자가 안보이는건 부모에 overflow:hidden; 설정을 했기 때문 → overflow지우고 높이를 설정해주기
### checked
* 사용자가 체크박스 또는 라디오 버튼을 선택했을 때 상태에 따라 디자인을 변경,적용
* input type=”checkbox” name=”ck” value=”ck1”
* input type=”radio” name=”ck” value=”ck2” id=”ck2”
* value 서버전송값  id→label과 연결
 * label for=”ck2”>로그인 상태유지</label>
* input[type^=check]:checked {color:pink;}
* input[name^=ck]:checked ~label {color:red;} input이 체크되었을 때 뒤에 형제 모든 라벨에 빨강을 하겠다
* ~ 뒤에 모든 형제   /  + 바로 다음 형제
## 속성선택자
* html요소 중 주로 form 관련 요소에 사용하는 선택자로 속성 (attribute)을 기준으로 스타일을 적용한다. [] 대괄호 속성명,속성값 등을 기준으로 요소를 선택한다
* 통일된 값
 * [속성]   속성이 존재 시 선택
 * [속성=값]  속성과 값이 정확이 일치 시 선택
 * [속성^=값]  속성의 값이 이 것으로 시작하는 경우 선택
 * [속성$=값]  속성의 값이 이 것으로 끝나는 경우 → 통일된 게 없을 때는 하나만 잡겠다
 * [속성*=값]  속성의 값이 이것을 포함하는 경우
----
### 25/04/25
## form 태그 관련 속성 주요 뜻과 사용 용도
* 입력 양식 : `input type=` text, password, email, search, number 등...
* 선택 양식 : `input type=` checkbox, radio, select, option 등...
* 입력 양식과 선택 양식에 따라 같은 스펠링 속성의 뜻이 달라지므로 주의 
## 양식에 따라 다른 속성의 뜻
* `value` 입력양식(사용자가 입력한 값-속성 작성 X) / 선택양식(사용자가 선택해서 서버에 전송되는 값-속성 작성 필수)
* `name` 입력양식(사용자가 선택해서 서버에 전송되는 값) / 선택양식(1개도 가능-2개 이상의 선택양식을 묶어주는 동일 그룹) => 둘 다 작성 필수
* 입력양식에서 value의 초기값을 작성하는 경우 : 쇼핑몰의 주문수량(기본값 1)
## form 속성에 사용자정의값을 이름 작성할 경우 주의사항
* name, value, id, class 등 속성의 이름을 작성할 때는 **중복명칭_개별명칭**을 섞어서 작성한다.
* 중복명칭에서 주로 사용하는 단어 : `admin, user`
* 개별명칭은 요소 특징에 따라 달라진다.(`main, id, btn, pw` 등)
* 중복명칭 설정 시 작성방향도 동일하게 해야한다.
* `user_id == user_pw` O
* `user_id == pw_user` X
## 목록양식 select, option (선택목록이 2개 이상일 경우)
* 기존목록과 비교해서 외우기 select(ul), option(li)
* `select`태그는 option을 묶어주는 그룹개념으로 그룹 속성(name)이 함께 적용된다.
* `option`태그는 사용자가 실제 선택하는 값이므로 데이터 구분값 속성(value)을 작성한다.
* `option`태그 작성 시 모든 value속성은 필수가 아닌 사용자가 선택되는 데이터에만 사용한다.
* 선택 option -> 1.컬러(value x) 2.블랙(black) 3.화이트(white) 4.코랄(coral)
## 선택양식 radio, checkbox 주의사항 label 주의사항
* radio, checkbox는 name(동일그룹), value(개별 데이터값) 속성을 구분해서 사용한다.
* `id`속성을 사용할 때는 `자바스크립트`와 연결을 위해서 하거나 또는 label의 `for`속성 연결을 위해서 사용한다. 이때 id값은 기존 개별데이터값을 가진 `value`와 동일한 값을 작성해도 된다.
* `label`은 사용자가 선택하는 이미지 또는 글자를 묶어서 작성하고 기존 선택양식 input의 형제로 작성한다면 반드시 `for`속성을 입력해서 input의 id와 동일하게 입력하고, 반대로 input의 부모로 작성한다면 for을 입력하지 않아도 된다.(=>생략가능 / 쓰면안된다 X) 대신 이 경우엔 선택하는 이미지 또는 글자를 반드시 다른 인라인 태그로 묶어야 한다.
* input radio, checkbox는 사용자커스텀 css 디자인이 불가능하기 때문에 사이트에 어울리는 모습으로 디자인하고 싶다면 `display:none`으로 숨기고 선택글자를 묶은 태그에 `backgorund-image`로 디자인해야 한다.
### input과 label이 형제인 경우
* `<input id="a"><label for="a">선택글자</label>`
### input과 label이 부모-자식인 경우
* `<label><input id="a"><span>선택글자</span></label>`
## button 속성 종류와 사용처
* `<button type="속성종류" id="버튼구분명">보이는글자 or 이미지</button>`
* 속성종류 1. button : 범용기능(주소찾기, 중복확인, 이전, 다음, 재생, 정지 등)
* 속성종류 2. submit : `form action`주소에 `method`값 형태로 전달되는 최종 서버전송버튼
* 속성종류 3. reset : 취소 or 삭제 버튼(가입취소, 주문취소 등)
----
### 2025/04/28
## css calc() 함수
* css에서 길이, 비율, 수치 등을 게산할 때 사용하는 함수
* 단위가 다른 (px,% 등) 값도 계산할 수 있어서 레이아웃 조정 시 유용함
* `+,-,*,/` 산술 연산자 모두 사용 가능
* 계산 시 **연산자 앞 위 반드시 공백포함**해서 작성하기
### css calc() 함수 예시
* `height:calc(50vh -100px);` 사용자가 보는 화면의 50크기 - 100px
* `padding:calc(100% - (10px * 3));` 우선순위 괄호 추가 사용 가능 | 10px을 *3(숫자만 들어가면 요소의 개수를 뜻함)해서 100%에서 뺀 값을 padding에 적용한다
* `width:calc(90% - (60px + 5px));` 우선순위도 연산자 앞,뒤 공백 필수 | 60과 5가 다른 요소에 들어 있어서 풀어서 적기도 함
* `width:calc(90% - 65px);` 
## Flex Layout
* 메인축 : 아이템이 정렬된 방향
* 교차축 : 아이템이 교차된 방향
* flex는 수평, 수직 1차원 레이아웃으로 메인축과 교차축을 고려하여 다양한 레이아웃을 만들 수 있는 CSS3의 새로운 레이아웃 속성이다.
* container(부모속성), item(자식속성)에 주는 속성이 다르기 때문에 주의해서 작성. **기본시작은 부모**
* `dispaly:flex` 부모(container)대상에 dispaly 명령어로 해당 레이아웃이 flex라는 선언부터 시작한다.
* (위) flex 선언을 진행 시 메인축은 기본값 수평, 교차축은 기본값 수직으로 정렬된다.
* (reverse -> 역순)
* `flex-direction:row;` 수평으로 정렬
* `flex-direction:column;` 수직으로 정렬
* `flex-wrap:wrap;` 자동줄바꿈
* `flex-wrap:nowrap;` 줄바꿈 X (기본값)
* `flex-flow:row wrap;`
* `justify-content:flex-start;` 왼쪽으로 정렬 -> row-reverse와 비슷하지만 역순이 아님
* `justify-content:flex-end;` 오른쪽으로 정렬
* `justify-content:center;` 가운데 정렬
* `justify-content:space-between;` 첫째와 막내는 양쪽 끝으로 정렬, 나머지는 균등배치 (부모의 끝에 배치가 우선순위)
* `justify-content:space-around;` 자식들을 균등하게 배치 (자식의 여백이 우선순위로)
* **justify는 메인축 정렬** -> row / column에 따라 정렬이 달라짐.
----
### 25/04/29
## Flex
* **align는 교차축 정렬**
* 교차축 2줄 이상일때 정렬방법 (flex-wrap:wrap 기준)
* `align-content:flex-start;` 
* `align-content:flex-end;`
* `align-content:center;`
* `align-content:space-between;`
* `align-content:space-around;`
* 교차축 1줄 이상일때 정렬방법 (flex-wrap:nowrap 기준)
* `align-items` start,end,center
* **item에 적용하는 속성**
* `align-self` start,end,center (교차축 1줄이상)
* `order` -> 음수부터 양수까지 작은수에서 큰수로 정렬이 적용된다. (중간에 비워지는 숫자 없이 값 적용하기)
* `flex` 부모에 크기에 반응해서 비율적용 (메인축 기준)
----
### 25/04/30
## Position
### 필수속성 relative, absolute, fixed, sticky
### 선택속성 top, bottom, left, right
* `flex, float` 등 포함 위치가 잡혀있는 요소에서 상/하/좌/우로 살짝 이동을 할 때는 `position:relative;`
* 형제요소 또는 부모-자식 요소 관계에서 부모 원리를 기준으로 요소를 겹치거나 현재 위치와는 관계없이 멀리 이동할 경우는 `position:absolute;`
* **주의사항** `absolute`사용 시 부모들 중 별도의 position 속성이 없다면 `body`를 기준으로 위치가 설정되니 부모 중 원하는 기준 대상에 반드시 position 속성을 함께 작성해야한다. `absolute, fixed, sticky` 모두가능!(상황에 따라 조합하기)