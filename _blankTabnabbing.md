# \_blank 속성을 이용했을때 Tabnabbing 공격

target 속성중 \_blank라는 속성이 있다  
이 속성은 링크를 클릭했을때 연결문서를 새로운 윈도우나 탭에서 오픈하는 속성이다

이렇게 새로운 페이지를 오픈하면서 tabnabbing 이라는 공격이 들어올수 있다

### tabnabbing 이란 ?

Tabnabbing이란 속성이 \_blank인 링크를 클릭했을때 열린탭에서 기존문서의 location을 피싱사이트로 변경해 정보를 탈취하는 공격기술을 말한다
![title](https://blog.coderifleman.com/images/tabnabbing_attack_and_noopener/tab-nabbing.01.svg) 1.사용자가 cgm.example.com에 접속한다  
2.해당 사이트에서 happy.example.com으로 갈 수 있는 외부 링크를 클릭한다.  
3.새탭으로 happy.example.com가 열린다  
happy.example.com에는 window.opener 속성이 존재한다(자신을 오픈한 부모창을 제어할수 있는 속성)  
자바스크립트를 사용해 opener의 location을 피싱 목적의 cgn.example.com/login 으로 변경한다  
4.사용자가 원래 탭으로 돌아오고 사용자는 로그인이 풀렸다고 생각하며 아이디 비밀번호를 입력한다  
이런식으로 정보를 탈취하는것을 tabnabbing 이라 한다

### 어떻게 막을수 있을까??

Gmail은 Anchor태그에 data-saferedirecturl 속성을 부여해 안전하게 리다이렉트한다

#### `rel=noopenr`속성

이 속성이 부여된 링크를 통해 열린페이지는 location 변경과 같은 자바스크립트 요청을 거부한다 (Uncaught TypeError를 발생시키면서) 또한 이 속성을 사용해 열린 탭은 부모를 호출할 일이 없기 떄문에 새 페이지가 느리다고 부모탭까지 느려질 일도 없다
