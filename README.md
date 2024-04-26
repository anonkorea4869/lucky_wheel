# 돌림판 이벤트 팔로워 자동 크롤러
정직하게 돌림판 이벤트를 하려는데 팔로워를 입력하기 힘든가요? 그러면 해당 프로그램을 사용해보세요!

## 성능
100명 찾는데 약 8초, 1만명의 경우 약 13분이 소요됩니다.

## 동작 원리
selenium 등으로 브라우저를 키지 않아도 팔로워 목록 확인할 때의 request를 분석하여 팔로워를 계속 가져옵니다.

## 파일 다운로드 방법
1. 상단에 main.py를 클릭합니다.
2. 우측에 Raw 두칸 옆에 있는 다운로드 버튼을 클릭합니다.

## 사용 방법
### 사용자 넘버, 쿠키 가져오기
**- 사용자 넘버 : 팔로워를 찾을 사용자의 교유 식별자(숫자)를 알아내야합니다.**

**- 팔로워 목록은 로그인해야만 볼 수 있으므로 로그인 정보가 있는 쿠키 수동으로 가져와야합니다.**

1. 인스타그램을 키고 로그인 합니다.
2. 크롬에서 개발자 도구를 켜줍니다.(Window : f11, Mac : option + mac + i)
3. 상단 부분에 애플리케이션(Application)을 클릭합니다.
4. 좌측에서 쿠키를 찾아주고 "https://www.instagram.com" 으로 시작하는 글자를 클릭합니다.
5. **ds_user_id**와 **sessioniod**에서 값 영역을 클릭해서 따로 보관합니다.

### Windows OS 실행 방법
6. 파일 탐색기를 통해 **main.py**를 찾습니다.
7. 상단 부분을 클릭하고 **cmd**를 입력해줍니다.

### MAC OS 실행 방법
6. finder를 통해 **main.py**를 포함하는 폴더를 찾습니다.
7. 폴더를 우클릭하여 '폴더에서 새로운 터미널 탭 열기'를 클릭해줍니다.

### 이후 공통
8. 새로운 창이 뜨면 **python3 main.py**를 입력한 후 엔터를 눌러줍니다.  
8-1. 만약 python이 없어 실행되지 않으면 개인적으로 다운로드 받습니다.
9. ds_user_id 입력 창이 뜨면 따로 보관했던 문자열을 붙여넣어줍니다.
10. sessionid 입력 창이 뜨면 따로 보관했던 문자열을 붙여넣어줍니다.
12. '총 n명 팔로워를 찾았습니다.' 문자열이 뜨는것을 확인합니다.(인스타그램에서 표시되는 팔로워 수와 마지막 문구에서의 팔로워 수는 다를 수 있지만 프로그램 문구가 올바릅니다.)
13. '팔로워 목록이 현재시간.txt 이름으로 저장되었습니다.' 문구가 뜰때까지 기다립니다.(기다리는 동안 다른 작업 가능)
14. main.py와 같은 위치에 현재시간으로 파일이 생성되는데 파일 내용을 복사 붙여넣기 등으로 사용하시면 됩니다.

## 출력 양식
파일에 출력되는 양식은 id, id, id입니다. 만약 양식이 마음에 들지 않으면 직접 코드 수정 혹은 인스타그램(@kimdaehun4869)로 DM주세요.
- 형식 맞춰 사용 가능한 돌림판 사이트 : https://ohmyluck.com/ko/

## 주의
만약 해당 기능이 웹사이트로 구현되어있다면 이는 개발자가 여러분의 로그인 정보를 가져갈 수 있으니 사용하지마세요.