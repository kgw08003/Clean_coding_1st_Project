###  🚀Clean_Curly 프로젝트 1st 🚀
- 마켓컬리 백엔드 클론코딩 프로젝트.
- 이커머스 사이트의 필수 기능을 구현
- 1차 프로젝트 결과임으로 아직 완벽하게 완성된 버전은 아님


### 🚴개발 인원 및 기간
- [팀프로젝트 기간] 2024-09.02(월) ~ 2024-09.13(금)
- [개발인원] : 백엔드 4명

### 🛠️기술스택
- Language : `python3`
- Framework : `Django`

### 💡ERD(1st)
![image](https://github.com/user-attachments/assets/2bcc12f3-f569-4b35-812c-f2b53c66e4c5)


### 🤗 팀 멤버
- [신덕근](https://github.com/shindeokgeun)
- [김향은](https://github.com/myangeun)
- [김혜지](https://github.com/hjkim977)
- [김지웅](https://github.com/kgw08003)

### 홈페이지 데모
![클린컬리](https://github.com/user-attachments/assets/bd02c593-fa10-48bb-979d-a24f744183ea)


### 📃 구현 기능📃 

#### 김지웅
- [`ERD` 내 `USER` 기능 담당]
- 회원가입 및 유저 관련 내용 로그인 페이지
- 로그인
![image](https://github.com/user-attachments/assets/0e599038-ebb7-4f53-a9cf-77babee87063)
- 회원가입
![image](https://github.com/user-attachments/assets/5c82ea31-0d02-46f7-ac5b-cee173fb1056)

- 로그아웃시 메인 홈페이지 이동
- 개인 정보 페이지(`users` 내 비밀번호 재확인 페이지, 개인정보 페이지(유저정보 관련 내용)
  
- 비밀번호 재확인 페이지
![image](https://github.com/user-attachments/assets/f87e64ca-d6d7-4f37-a2b6-4a0e363e3de8)

- 개인정보 페이지
![image](https://github.com/user-attachments/assets/3216e47e-51e1-437a-9877-36062881d80e)

- 홈페이지 메인 화면 구축(html, css)
- 특가/혜택, 고객센터 기본 구축

### 🔐 코드 작성하면서 어려웠던 기능🔐
###### CSS 디자인 조정의 어려움
- 문제점: 새로운 기능을 추가할 때마다 CSS 디자인이 미세하게 맞지 않아 어려움을 겪었고, 주로 `margin`과 `padding`을 통해 조정하였지만 정확한 조정이 어려웠음.
- 해결 방법: 여러 번의 시도 끝에 디자인을 시각적으로 적절하게 맞출 수 있었고, 특히 메인 홈페이지의 배너 슬라이드 기능에서 스크립트를 사용해 3초마다 배너가 넘어가도록 구현함. 하지만, 페이지 크기를 조절할 때 배너 크기가 적절히 조정되지 않는 문제가 여전히 남아있음.

###### 비밀번호 재확인 폼의 입력란 잠금 기능
- 문제점: 사용자 프로필에 들어가기 전에 비밀번호를 재확인하는 폼에서, 아이디 입력란을 잠그고 싶었음.
- 해결 방법: `readonly` 속성을 사용하여 입력 필드를 수정할 수 없게 만들었음. `readonly` 속성은 HTML의 `<input>` 요소에서 사용자가 값을 수정하지 못하도록 설정하는 속성으로, 보안과 사용자 편의성을 동시에 달성할 수 있었음.
- ```<input type="text" name="id" value="{{ user.username }}" readonly class="readonly-input">```


###  📝구현하려 했으나 해결하지 못한 기능📝
###### 선물특가 타이머 기능
- 메인페이지 타이머 기능을 구현할 때, 새로고침을 해도 타이머가 흐른 시간을 유지하도록 하려고 했으나, 시간이 한번 설정되면 수정이 불가능한 문제가 발생했음. 새로고침 후에도 타이머가 초기화되지 않고 흐른 시간이 유지되도록 하는 것이 어려웠음.
- 현재 상태: 결국 타이머는 새로고침 시마다 시간이 초기화되는 방식으로 설정되었으며, 해당 문제는 3차 프로젝트에서 해결할 계획임.

### 🔥2차 프로젝트에서 구현하고 싶은 기능🔥
###### 개인 페이지에서 회원 정보 및 비밀번호 수정 기능
- 사용자들이 자신의 회원 정보를 수정할 수 있는 기능을 추가하고 비밀번호를 변경할 수 있는 기능을 함께 구현하여 사용자 경험을 개선하고, 보안을 강화할 예정.

###### 추천인 코드 및 마일리지 기능
- 추천인 코드를 통해 새로운 회원 가입 시 추천한 사용자에게 마일리지를 적립해주는 기능을 구현할 예정임. 이 기능을 통해 사용자들의 참여를 독려하고, 마일리지를 활용해 다양한 혜택을 제공할 수 있도록 할 계획임.

###### 홈페이지 검색어 입력 기능 연동
- 사용자가 검색어를 입력하면 해당 검색어에 맞는 상품이나 정보를 연동하여 제공하는 검색 기능을 추가할 예정임.


### 실행 방법 ⚙️
##### 패키지 설치
```  images파일 추가
python -m venv myweb
만들어진 폴더에 zip 파일내용 붙여넣기
cd myweb
./Scripts/activate

pip install django djangorestframework
pip install django_extensions pillow
또는 pip install -r requirements.txt 이용
python manage.py runserver
```
