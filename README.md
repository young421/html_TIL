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