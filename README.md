<img src="http://www.logobird.com/wp-content/uploads/2011/01/New-HTML5_Logo.png" width="1000" height="400">

# HTML 시작

## HTML 기본구조

```
<!DOCTYPE html>
<html>
    <head>
        <title>HRML 문서의 제목입니다. </title>
    </head>
    <body>
        <h1>가장 큰 제목크기 입니다.</h1>
        <p>단락을 적는 부분</p>
    </body>
</html>
```

#### `<!DOCTYPE html>` : 현재문서가 HTML5 문서라는것을 알려줍니다.

#### `<title>` : 문서의 제목을 정의하며 웹문서 툴바에 표시됩니다.

#### `<body>` : 웹 브라우저를 통해 보이는 내용 부분입니다.

#### `<h1>`~`<h6>` : 제목을 나타낸다 h1이 가장크고 h6이 가장 작습니다.

#### `<p>` : 단락을 나타냅니다.

***

## HTML 요소구조

#### HTML 요소는 여러속성을 가질 수 있으며 속성은 해당요소에 대한 추가적인 종보를 제공합니다.
#### 또한 HRML 요소는 시작태그 `<>` 시작해 종료태그 `</>` 로 끝납니다.
![image](https://user-images.githubusercontent.com/81845425/128367670-816bf894-3a77-4ec5-861b-6cc435789c68.png)
#### 속성은 HTMl 요소 중에서도 언제나 시작태그 내에서만 정의되고 속성 이름과 속성값을 표현됩니다.
```<태그이름 속성이름 ="속성값">```

***

# HTML 텍스트 요소

## 제목

#### HRML은 제목을 표현할 수 있는 `<h>`태그를 제공합니다.
#### 가장큰 `<h1>` 부터 가장 작은 `<h6>` 태그로 제목크기를 정할수 있습니다.
```
<h1>제목1의 크기입니다</h1>
<h2>제목2의 크기입니다</h2>
<h3>제목3의 크기입니다</h3>
<h4>제목4의 크기입니다</h4>
<h5>제목5의 크기입니다</h5>
<h6>제목6의 크기입니다</h6>
```
## 단락

###단락
#### 단락이란 끊어서 구분할수 있는 하나하나의 분을 의미하며 , 문단이라거더 부릅니다
#### HRML 에서는 `<p> 내용 </p>` 태그를 이용하여 단락을 표현합니다.
```
<p>단락 입니다.</p>
```
### 줄 나누기

#### HTML 코드에서 띄어쓰기나 줄 나누기를 여러 번 하더라도 실제 화면에서는 전혀 영향을 주지 않습니다.
#### 웹브라우저는 여러번의 띄어쓰기나 줄 나누기를 오직 하나의 띄어쓰기나 줄로만 인식하기 때문입니다.
#### 줄내리기를 하기 위해서는 `<br>`태그를 사용합니다. 
```
<p>
줄<br>
나누기<br>
이렇게 줄을 나눠봤습니다.<br>
</p>
```
### 텍스트 서식 미리 정의하기

#### HTML 코드에 작성한 그대로를 웹문서에 표현하기 위해서는 `<pre>` 태그를 사용해야합니다.
#### `<pre>` 태그는 HTML 문서에 작성된 모든 띄어쓰기와 줄나누기등을 그대로 웹문서에 표현해 줍니다.
```
<pre>

줄을 나누

기

이렇게 줄을 나눠
  봤습니다.

     그대로     출력     

</pre>
```
### 수평 가로 구분선

#### 단락을 나눌때나 내용구분을 하기위해서 수평가로 구분선을 사용합니다
#### 수평 가로 구분선은 `<hr>` 태그로 만들수 있습니다.
```
<p>단락입니다.</p>
<hr>
<p>단락.</p>
```
## 서식

### 강조 효과

#### 텍스트를 굵게 표현하고 싶을떄는 `<b>` 태그 나 `<strong>` 태그를 사용합니다
`<p>가나다라<b>마</b>바사아자차카<strong>파</strong>타하</p>`

#### 텍스트를 이탤릭체로 표현하고 싶을때는 `<i>` 태그나 `<em>`태그를 사용합니다.
`<p><i>이탤릭체</i></p>`

#### 하이라이팅 효과를 적용시키고 싶을 떄는 `<mark>` 를 사용합니다.
`<p><mark>"이 부분"</mark>하이라이팅</p>`

#### 텍스트를 지운것과 같은 효과를 내게 하고 싶을 떄는 `<del>` 태그를 사용합니다.
`<p><del>"이 부분"</del>지운부분.</p>`

#### 텍스트 밑에 가로줄을 만들어 텍스트를 삽입한 것과 같은 효과를 내주고 싶을 떄는 `<ins>` 태그를 사용합니다.
`<p><ins>"밑줄 친 부분"</ins>에 들어갈 알맞은 말을 고르세요.</p>`
***

## 인용구

### 짧은 인용구

#### 짧은 인용구는 `<q>` 태그를 이용하여 표현할수 있습니다.
`<p>HTML의 정의는<q>웹 페이지를 만들기 위한 하이퍼텍스트 마크업 언어</q>입니다.</p>`

### 블록 인용구

#### 길이가 긴 인용문은 `<blockquote>` 태그를 이용하여 표현 할 수 있습니다.
```
<p>HTML의 정의</p>
<blockquote>
인터넷 서비스의 하나인 월드 와이드 웹을 통해 볼 수 있는 문서를 만들 때 사용하는 프로그래밍 언어의 한 종류이다.
</blockquote>
```

### 축양형 표현

#### HTML에서 용어의 축양형을 표현하기 위해서는 `<abbr>` 태그를 사용합니다.
#### `<abbr>` 태그에 마우스를 가져가면 title 속성에 적은 것이 나타납니다.
```
<p><strong><abbr title="HyperText Markup Language 5">HTML5</abbr></strong>
란 웹 문서를 제작하는 데 쓰이는 프로그래밍 언어인 HTML의 최신규격입니다.</p>
```

### 주소 표현

#### `<address> `태그를 사용해 자신의 주소를 표현할수 있습니다.
#### 주소는 이탤릭체로 표현되며 공백이 자동으로 삽입됩니다.
```
<address>
    대구광역시<br>
    동구
</address>
```
***

## 스타일

#### HTML 요소의 `<style>` 속성을 이용하면 CSS 스타일을 HTML 요소에 직접 설정할수 있습니다.
`<태그이름 style="속성이름:속성값">`

### 배경색 변경

#### `style="background-color:"`를 이용하여 자신이 원하는 배경색으로 설정할수 있습니다.
```
<h1 style="background-color:white">
   배경색 변경
</h1>
```

### 글자색 변경

#### `style="color:"`를 이용하여 자신이 원하는 글자색을 설정할수 있습니다.
```
<h1 style="color:green">
    글자색 변경
</h1>
```

### 글자 크기 변경

#### `"font-size:"`를 이용하여 글자크기를 설정할수 있습니다.
```
<h1 style="font-size:450%">
  글자 크기 변경
</h1>
```

## HTML 링크

#### 웹페이지에는 다른 페이지나 사이트로 연결되는 하이퍼링크가 존재 합니다.
#### 이러한 링크를 HTML에서는 `<a>` 태그로 표현합니다.
`<a href="링크주소">HTML 링크</a>`

#### `<a>` 태그에는 여러가지 속성이 있습니다.
![target](https://user-images.githubusercontent.com/81845425/128633827-d44ee209-09cf-482d-966d-83d19103edc8.png)

## HTML 이미지

### 이미지의 삽입

#### HTML문서에 이미지를 삽입할때는 `<img>` 태그를 사용합니다.
`<img src="이미지주소" alt="대체문자열">`
#### src는 이미지의 주소를 나타내고 alt는 이미지가 로딩될때 동안 나오는 글자 입니다.

### 이미지의 크기 설정

#### HTML에서 width와 hright를 사용하여 이미지의 크기를 설정할수 있습니다.
#### width는 너비 hright는 높이를 나타냅니다.
```
<img src="/examples/images/img_flag.png" alt="html size" width="320" height="214">
<img src="/examples/images/img_flag.png" alt="style size" style="width:320px; height:214px">
```

### 이미지에 링크설정

#### 이미지에`<a>`태그를 이용하여 링크를 설정할 수 있습니다.
```
<a href="/html/intro" target="_blank">
    <img src="/examples/images/img_flag.png" alt="flag" style="width:320px; height:214px">
</a>
```
***
## HTML 리스트

### 순서가 없는 리스트

#### 순서가 없는 리스트는 `<ul>` 태그로 시작하며 포함되는 각각의 요소는 `<li>`태그로 시작합니다.
```
<ul>
    <li>가</li>
    <li>나</li>
    <li>다</li>
</ul>
```

### 순서가 있는 리스트

#### 순서가 있는 리스트는 `<ol>`태그로 시작하며 포함되는 각각의 리스트 요소는 `<li>`태그로 시작합니다.
```
<ol>
    <li>가</li>
    <li>나</li>
    <li>다</li>
</ol>
```

### 정의 리스트

#### 정의리스트는 용어와 그에 대한 정의를 모아놓은 리스트로 `<dl>` 태그로 시작합니다.
#### `<dt>` 태그에는 용어이름, `<dd>` 태그에는 용어에 대한 정의가 들어갑니다.
```
<dl>
    <dt>용어1</dt>
    <dd>- 설명</dd>
    <dt>용어2</dt>
    <dd>- 설명</dd>
</dl>
```
***
## HTML 표(태이블)

### HTML 테이블

#### `<table>`태그는 `<tr>`,`<th>`,`<td>`태그로 구성됩니다.
#### 1.`<tr>` 테이블에서 열을 구분 해줍니다.
#### 2.`<th>` 각 열의 제목을 나타냅니다.
#### 3.`<td>` 열을 각각의 셀로 나누어 줍니다

```
<table>
    <tr>
        <th>참치</th>
        <th>고래</th>      
    </tr>
    <tr>
        <td>상어</td>
        <td>문어</td>
    </tr>
    <tr>
        <td>오징어</td>
        <td>고등어</td>
    </tr>
</table>
```

### 테이블의 열 합치기

#### `colspan` 속성을 이용하면 테이블의 열을 합칠수 있습니다.
```
<table>
    <tr>
        <td>참치</td>
        <td colspan="2">고래</td>        
    </tr>
    <tr>
        <td>상어</td>
        <td>문어</td>        
        <td>꽁치</td>
    </tr>
</table>
```

### 테이블의 행 합치기

#### `rowspan` 속성을 사용하 행을 합칠수 있습니다.
```
<table>
    <tr>
        <td rowspan="2">상어</td>
        <td>문어</td>        
        <td>꽁치</td>
    </tr>
    <tr>
        <td>고등어</td>        
        <td>돌고래</td>
    </tr>
</table>
```

### 테이블의 캡션 설정

#### `<caption>` 태그를 사용하면 테이블 상단에 제목이나 짧은 설명을 적을수 있습니다.
```
<table>
    <caption>해양 생물</caption>
    <tr>
        <td>참치</td>
        <td>고래</td>
        <td>날치</td>    
    </tr>
</table>
```
***
## iframe 요소

### iframe 요소
#### iftame 요소를 이용하면 웹페이지안에 또 다른 웹페이지를 삽입할 수 있습니다.
`<iframe src="삽입할페이지주소"></iframe>`
***
## Form 요소

### from 요소
#### 웹페이지에서는 `form` 요소를 사용하여 사용자로 부터 입력을 받을수 있고 
#### 사용자가 입력한데이터를 서버로 보낼때도 `form` 요소를 사용합니다.
`<form action="처리할페이지주소" method="get|post"></form>`

#### `action` 속성은 입력받은 데이터를 처리할 서버상의 스크립트 파일의 주소를 명시합니다.

### method 속성

#### method 속성을 통해 명시할 수 있는 form 요소의 전달방식은 `GET` 방식과 `POST` 방식으로 나눠집니다.

#### `GET` 방식은 주소에 데이터를 추가하여 전달하는방식입니다. 
##### 크기가 작으며 종요도가 낮은 정보를 보낼때 주로 사용합니다.

#### `POST` 방식은 데이터를 별도로 첨부하여 전달하는 방식입니다.
#### 데이터가 외부에 드러나지 않고 데이터 크기제한이 없어 보안성 및 활용성이 `GET` 방식보다 좋습니다

### 다양한 input 요소

#### HTML에는
#### 1. 텍스트 입력(text)
#### 2. 비밀번호 입력(password)
#### 3. 라디오 버튼(radio)
#### 4. 체크박스(checkbox)
#### 5. 파일 선택(file)
#### 6. 선택 입력(select)
#### 7. 문장 입력(textarea)
#### 8. 버튼 입력(button)
#### 9. 전송 버튼(submit)
#### 10. 필드셋(fieldset)
#### 이러한 input 요소가 있습니다

### 텍스트입력

####  `<input>`태그의 type 속성값을 `"text"`로 설정하면
#### 사용자로부터 한 줄의 텍스트를 입력받을 수 있습니다.
```
<form>
    <input type="text" name="search">
</form>
```

### 비밀번호 입력

#### `<input>`태그의 type 속성값을 `"password"`로 설정하면
#### 사용자로부터 비밀번호를 입력받을 수 있습니다.
```
<form>
    사용자 : <br><input type="text"><br>
    비밀번호 : <br><input type="password">
</form>
```

### 라디오 버튼

#### `<input>`태그의 type 속성값을 `"radio"`로 설정하면
#### 사용자로부터 여러 개의 옵션 중에서 단 하나의 옵션만을 입력받을 수 있습니다.
```
<form>
    <input type="radio"> HTML <br>
    <input type="radio"> CSS <br>
    <input type="radio"> JAVA <br>
    <input type="radio"> C++
</form>
```

### 체크박스
#### `<input>`태그의 type 속성값을 `"checkbox"`로 설정하면
#### 사용자로부터 여러 개의 옵션 중에서 다수의 옵션을 입력받을 수 있습니다.
```
<form>
    <input type="checkbox"> HTML <br>
    <input type="checkbox"> CSS <br>
    <input type="checkbox"> JAVA <br>
    <input type="checkbox"> C++
</form>
```

### 파일선택
#### `<input>`태그의 type 속성값을 `"file"`로 설정하면
#### 사용자로부터 파일을 전송받을 수 있습니다.
```
<form>
    <input type="file" name="upload_file" accept="image/*">
</form>
```
#### accept를 이용하여 파일의 종류를 명시할수 있습니다.

### 선택 입력
#### `select` 요소는 여러 개의 옵션이 드롭다운 리스트로 되어 있으며
#### 그중에서 단 하나의 옵션만을 입력받을 수 있습니다.
```
<select name="fruit">
    <option value="apple"> 사과
    <option value="orange" selected> 귤
    <option value="strawberry"> 딸기
    <option value="peach"> 복숭아
</select>
```

### 문장입력

#### `textarea` 요소는 사용자로부터 여러 줄의 텍스트를 입력받을 수 있습니다.
```
<textarea name="message" rows="5" cols="30">
    여기에 적으세요.
</textarea>
```
#### `rows` 속성과 `cols` 속성을 이용하여 `textarea` 요소의 크기를 자유롭게 지정할 수 있습니다.

### 버튼

#### `button` 요소는 사용자가 누를수 있는 버튼을 나타냅니다.
```
<button type="button">
    버튼
</button>
```
### 전송 버튼
#### `<input>`태그의 type 속성값을 `"submit"`으로 설정하면
#### 사용자로부터 입력받은 데이터를 서버의 폼 핸들러로 제출하는 버튼을 만들 수 있습니다.
```
<form>
    <input type="submit" value="전송">
</form> 
```

### 필드셋
#### `fieldset` 요소는 form 요소와 관련된 데이터들을 하나로 묶어주는 역할을 합니다.
#### `legend` 요소는 `fieldset` 요소 안에서만 사용할 수 있으며 `fieldset` 요소의 제목을 나타냅니다.
```
<form>
    <fieldset>
        <legend>입력 양식</legend>
        이름 : <br>
        <input type="text" name="username"><br>
        이메일 : <br>
        <input type="text" name="email"><br><br>
        <input type="submit" value="전송">
    </fieldset>
</form>
```
***
## input 요소의 속성

### value 속성
#### `value` 속성은 `input` 요소의 입력 필드에 나타나는 초기값을 설정합니다.
```
<form>
    이름 : <br><input type="text" name="student_name" value="ex) 홍길동"><br>
    학번 : <br><input type="text" name="student_id" value="ex)1111"><br>
    학과 : <br><input type="text" name="department" value="ex)컴퓨터공학과"><br>
</form>
```

### readonly 속성

#### `readonly` 속성은 사용자가 입력 필드를 볼 수는 있으나, 수정할 수는 없도록 설정합니다.
```
<form>
    학과 : <br><input type="text" name="department" value="컴퓨터공학과" readonly><br>
</form>
```
### disabled 속성

#### `disabled` 속성은 사용자가 입력필드를 아예 사용할수 없도록 설정합니다.
```
<form>
    학과 : <br><input type="text" name="department" value="컴퓨터공학과" disabled><br>
</form>
```

### maxlength 속성

#### `maxlength` 속성은 입력필드에 입력할수 있는 최대 문자길이를 설정합니다.
```
<form>
    이름 : <br><input type="text" value="홍길동" maxlength="5"><br>
</form>
```

### size 속성

#### `size` 속성은 입력필드에 보여지는 input 요소의 크기를 설정합니다.
```
<form>
    size30 : <br><input type="text"  size="30"><br>
    기본 : <br><input type="text" ><br>
</form>
```
***
## 의미 요소
#### 의미요소란 그 자체로 의미를 가지고 있는 요소를 가리킵니다.
#### 즉 요소가 자기 스스로 브라우저와 개발자 모두에게 자신이 사용된 의미를 명확히 전달해주는 요소를 의미합니다.

### 의미 요소의 종류
![](http://tcpschool.com/lectures/img_html_html5_layout.png)

### header 요소

#### `header` 요소는 HTML 문서나 섹션 부번에 대한 헤더를 정의합니다.
```
<header>
    <h1>전체 문서에 대한 헤더(header)입니다.</h1>
</header>
<section>
    <header>
        <h2>섹션 부분에 대한 헤더(header)입니다.</h2>
        <p>헤더 부분에 들어간 단락입니다.</p>
    </header>
</section>
```

### nav 요소

#### `nav` 요소는 HTML 문서 사이를 탐색할 수 있는 링크의 집합을 정의합니다
```
<nav>
    <a href="/html/html5_element_semantic">의미 요소</a> |
    <a href="/htmlhtml5_element_form/">Forms 요소</a> |
    <a href="/html/html5_element_inputtype">Input 요소</a>
</nav>
```

### section 요소

#### `section` 요소는 HTML 문서에서 섹션 부분을 정의합니다.
#### HTML 문서의 전체적인 내용과 관련이 있는 콘텐츠들의 집합을 의미합니다.
```
<section>
    <h2>섹션 영역입니다.</h2>
</section>
```

### article 요소

#### `article` 요소는 HTML 문서에서 독립적인 하나의 기사 부분을 정의합니다.
```
<article>
    <h2>기사 영역입니다.</h2>
</article>
```

### footer 요소

#### `footer` 요소는 HTML 문서나 섹션 부분에 대한 푸터를 정의합니다
#### 푸터에는 사이트의 작성자, 그에 따른 저작권 정보, 연락처등을 명시합니다.
```
<footer>
    <p>전체 문서에 대한 푸터(footer)입니다.</p>
    <p>Copyright 2021. 지은이 000.</p>
    <p>연락처 : 010-1234-5678</p>
</footer>
```
