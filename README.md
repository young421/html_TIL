# HTML
### 250804 HTML시작
* 비주얼 스튜디오 코드 설치, 깃허브 회원가입, 깃 설치
* 비주얼  스튜디오 환경설정 및 플러그인 설치
### 주의사항
1. 영문 대소문자 사용하기(소문자 권장) 예) subTitle, sub_title
2. 숫자는 영문 뒤로 배치하기 예) sub1, main002
3. 공백 + 한글 사용금지
4. 특수문자 사용금지(#,$,%,^,&,*,(,+,\,~,★ 등..) *언더바(`_`) 하이픈(`-`) 가능
5. 이름은 의미있게 사용하기 예) images, fonts, mail, cafe 등..
6. 비주얼스튜디오코드 실행 시 작업 폴더 연결되어 있는지 확인하기
7. (위) 작업폴더 연결이 안 되어있다면 -> File -> Close Floder 후 다시 File -> Open Folder
### 깃(git) 설치 확인
* Vscode에서 단축키 `Ctrl + J` 터미널 실행
* `git -v` 깃설치버전 확인(버전결과가 나온다면 설치 ok)
### 터미널`Ctrl+J` 기본 설정
* 윈도우 기본 터미널 powershell을 사용하여 git Bash로 변경하기
* (위 gitBash는 깃설치 후 사용 가능)
## git 설정과 gitHub 업로드까지 순서(터미널 입력 기준)
1. `git config --list` : 현재 깃 설정 정보 확인
2. 새로운 값 입력 안 될 때는 터미널에서 `Ctrl+c` 또는 `Q`
3. 위 1번에서 깃 설정정보에 name, email이 내 정보가 아닐 때
4. `git config --global user.email "lucia042155@gmail.com"` 이메일 설정
5. `git config --global user.name "lucia042155"` 이름 설정(메일아이디 동일)
6. `git config --list` 위 4~5번 설정 올바르게 됐는지 확인
---
7. `git init` 현재 폴더를 작업 디렉터리 폴더로 연결, 폴더경로 옆에 **master**표시 생기면 성공!
8. `git branch -M main` 깃 디렉터리 명칭을 브랜치라 부름. 해당 브랜치명을 개인에 맞게 변경. 기본이 **main**
---
9. `git add .` **.**이란 작업수정한 모든 파일을 대기로(스테이지)에 올린다는 뜻 `git add README.md`
10. `git status` 현재 스테이지 확인 명령
11. `git commit -m "기록메세지"` 현재 올리는 파일이 어떤 내용인지기록
12. `git remote add origin 깃허브저장소주소` 깃허브 저장소 업로드 위치가 어디인지 주소 연결
13. `git push origin main` 11번에서 커밋한 파일을 12번 저장소에 최종 업로드하는 명령
### 한 번만 작성하면 끝인 깃 명령어
* `git config` 이름, 이메일 설정
* `git init` 저장소 설정
* `git branch -M main` 저장소 이름 설정
* `git remote add origin` 저장소 주소 설정
### 작업 시 깃허브 업로드를 위해 반복해야 하는 깃 명령어
* `git add .`
* `git commit -m '기록메세지'`
* `git push origin main`
* 필요시 중간 점검용으로 `git log` 또는 `git status`
# HTML 작성법
* `<태그속성="값" 속성="값"></닫기태그>`
* 시작태그부터 닫기태그까지 한 번에 **요소(element)**란 명칭으로 부른다.
* 속성은 시작태그에만 쓰고 닫기태그에는 속성을 쓰지 않는다.
* `파일명.html`
* 파일명은 **영문대소문자+숫자 조합**으로만 작성한다.
* HTML 작성의 시작은 항상 **구조태그**로 해야 한다! `html:5`
## Vscode 자주 쓰는 단축키
* `Ctrl+\` 화면 좌우 분할
* `Ctrl+K, \ ` 화면 상하 분할
* `Alt+Z` 자동 줄 바꿈
* `Alt+상하 방향키` 줄 이동
* `Shift+Alt+상하방향키` 선택한 줄 복제
* `Shift+Alt+A` 주석 생성
## 250805 자주 쓰는 HTML 문서 기본 태그
1. `<h1>~<h6>` block-1대제목~6소제목
2. `<p>` block-제목 아래 작성하는 내용태그
3. `<br>` inline-내용 안에 작성하는 줄바꿈태그
4. `<em><strong>` inline-내용 안 강조태그
5. `<del>` inline-쇼핑몰 원가 등에 사용하는 삭제태그
6. `<address>` block-회사 주소
7. `&copy;` 특수문자태그-copyright 약자
## 250806 레이아웃 태그 TIP
* `<div>` : 2개 이상의 블록 또는 인라인을 묶어주는 그룹, 작성과 동시에 반드시 **class 또는 id**를 의미있는 이름으로 작성해야 한다.
* `<div id="">` : id는 **반복되지 않는 고유한 이름**을 설정하고 바깥쪽 큰 레이아웃에 주로 사용한다.
* `<div class="">` : class는 **반복될 수 있는 이름**을 설정하고 바깥쪽부터 안쪽까지 다양한 레이아웃에 사용한다.
* `<span></span>` : 2개 이상의 인라인 요소를 묶어주는 그룹 또는 **디자인 구분을 위해 태그를 나눠야 할 때+형제가 인라인 요소일 경우** 의미가 없는 부분에 자주 이용한다.
* `class or id` : 클래스와 아이디 속성은 구분이 필요한 모든 태그에 추가로 작성할 수 있다. **태그에 2개 이상 연속적으로 작성되어 구분이 필요한 경우** 클래스를 주로 사용한다.
### 바로가기링크 준비
* 준비 대상) 클릭할 a 요소와 이동할 위치 요소(아이디 선언)
1. 이동할 위치에 중복되지 않는 명칭으로 아이디 설정
* `<태그 id=review_pst></태그>`
2. 위치로 이동하는 클릭 요소에 위 1번 아이디를 이용한 링크 설정
* `<a href="#review_pst"> 클릭 글자 또는 이미지</a>`
* `#이름` == 임시링크(x) 아이디(o)
* `#` == 임시링크(o) 아이디(x) 
### 바로가기 링크 다양한 사용 예
* 같은 페이지의 다른 위치로 이동 시
* `<a href="#위치아이디명">클릭요소</a>`
* 다른 페이지의 특정 위치로 이동 시
* `<a href="./상대경로#위치아이디명">클릭요소</a>`
* `<a href="./login.html#search">클릭요소</a>`
## git 버전관리
### gitHub 폴더 복제 방법
* `git clone 주소 붙여넣기`
### gitHub 수정된 작업물 내려 받기
* `git pull origin main`
---
# CSS 
## 캐스케이딩 스타일 시트(폭포 단계별로 작성하는 CSS)
### CSS 기초 작성 순서
1. `styles/reset.css` 파일 만들기
2. html 파일 head 안 `link:css` 자동 완성 작성하고 위 1번 파일 연결하기
3. (html 작성 완료 기준) 부모 -> 자식 순서대로 모든 선택자 작성하기 `{}` 중괄호 비운 상태로 
4. 모든 선택자 작성 후 `{속성:값;}` 추가로 작성하며 디자인 진행하기
# CSS 글자 속성
## font-family
* `font-family:'대표 글꼴', 후보글꼴, 글꼴유형`
* 글꼴유형 : sans-serif, serif
* 글꼴명에 한글, 특수문자, 공백이 있을 경우 '' 따옴표 묶기
* 윈도우 기본 설치 글꼴 : 굴림, 고딕, 바탕, 궁서
*  **대표 글꼴이 설치가 필요한 글꼴일 경우** : 해당 글꼴 파일을 웹주소로 연결해서 누구나 볼 수 있게 설정한다.
* `<link rel="stylesheet" as="style" crossorigin href="https://cdn.jsdelivr.net/gh/orioncactus/pretendard@v1.3.9/dist/web/static/pretendard-dynamic-subset.min.css" />`
## font-size
* 16px 평균값 기준으로 피그마, 포토샵 등에서 디자인한 글자 크기를 `rem, em` 단위로 변환해서 작성한다.
* 16px == 1em or 1rem
* `https://nekocalc.com/px-to-em-converter` 글자 변환 사이트
## HTML - Form
* 사용자 입력 / 선택 요소 1개라도 등장 시 전체 영역을 `form` 묶어주기 **action, method, id** 필수!
* 폼 안쪽 양식 종류가 그룹 별로 2개 이상 구분될 경우 `fieldset, legend` 작성한다.
* `fieldset` div처럼 그룹 역할이므로 id 또는 class를 함께 작성해야 한다.
* `fieldset` 생략하고 대신 `div, ul, ol, dl` 등 다른 그룹으로 대체하는 것도 가능하다.
### form - input
* `<input type="종류" name="데이터명(중복x)" id="데이터명(중복x) class="공통디자인명">`
* `value` 속성은 필요한 경우만 작성, 쇼핑몰 수량 1 기본값
## CSS Margin & Padding 작성 방법
* `1px 2px 3px 4px` : 위 -> 오른쪽 -> 아래 -> 왼쪽
* `1px` : 상하좌우 값 동일
* `1px 2px` : 상하(1) 좌우(2)
* `1px 0 2px` : 상(1) 좌우(0) 하(2)
* Margin 겹침 현상 주의!!