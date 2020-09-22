# **HTML Practical Page** - by suna jung

## **프로젝트 설명과 고찰**
> HTML의 개념과 태그에 관한 수업을 듣고 만든 실습 페이지입니다.

<br>

## **HTML 기초** 
---
<br>

### **[ HTML 기본 용어 ]**

<br>

- `tag` : HTML 페이지에서 객체를 만들 때 사용 
- `element` : 태그를 사용해 만들어진 객체
- `attribute` : 태그에 정보를 추가할 때 사용

    (ex) h1옆에 class 속성

``` html
<h1 class="title>HTML5 is Easy</h1>
```

- `comment` : HTML 코드를 설명하기 위해 작성, **'<\!-- -->'** 사이에 작성
<br><br>

### **[ HTML 페이지 구조 ]**

<br>

- `!doctype` : HTML 버전 스펙 명시

- `html 태그` : 모든 HTML 페이지의 루트 요소로 lang속성에 사용하는 언어 설정
 
 - `head 태그` : meta, title, script, link, style, base등 HTML 페이지의 여러 정보 제공

 - `body 태그` : 실제 사용자에게 보여지는 내용을 작성하는 부분

   > **tip: 빈 화면 - '!' 누른 후 엔터 - 필요없는 meta 정보 지워주고 lang ="ko"로 바꿔서 기본 환경 만들기.**

   <br>

<br>

## **기본 태그** 
---
<br>

### **[ 글자 관련 태그 ]**

<br>

- `제목<sup>header</sup> 태그` : h1 ~ h6

- `본문 관련 태그` : p(단락), br(줄바꿈), hr<수평줄>

- `글자 형태 관련 태그` : b(굵은 글자), i(기울어진 글자), small(작은 글자), sub(아래첨자), sup(윗첨자), ins(밑줄), del(취소선)

- `앵커<sup>anchor</sup> 태그` : 페이지 내에서 다른 위치, 혹은 다른 웹페이지로 이동할 때 사용. a 태그의 href 속성값으로 설정.
``` html
  <p> <!--다른 html로 이동-->
    <a href="./anchor.html">앵커 태그</a>
  </p>
  <p>  <!--다른 사이트로 이동-->
    <a href="http://naver.com">네이버</a>
  </p>
```
   > **tip: 공백 문자는 하나만 입력된 것으로 처리되며, 줄바꿈이 적용되지 않으므로 '\<br\>' 태그를 이용해야 함.**

<br>

### **[ 목록 관련 태그 ]**

<br>

- `ul` : 순서가 없는 목록

- `ol` : 순서가 있는 목록

- `li` : ul 또는 ol 태그 내부에서 사용, 목록의 아이템들을 나타내는 태그

``` html
<ul> <!--순서가 없는 리스트-->
  <li>아이템 1</li>
  <li>아이템 2</li>
  <li>아이템 3</li>
</ul>

<ol>  <!--순서가 있는 리스트-->
  <li>아이템 1</li>
  <li>아이템 2</li>
  <li>아이템 3</li>
</ol>

```
<br>

### **[ 표 관련 태그 ]** - table tag


<br>

 | 태그 이름 | 설명 | 속성 |
 |---|:---:|---:|
 | `caption` | 표의 제목을 작성하기 위한 태그 |  |
 | `thead` | 표의 헤더를 만들기 위한 태그 |  |
 | `tbody` | 표의 몸체를 만들기 위한 태그 |  |
 | `tfoot` | 표의 푸터 <sup>footer</sup>를 만들기 위한 태그 |  |
 | `tr` | 표의 행을 생성하는 태그 | `rowspan`, `colspan` |
 | `th` | 표의 제목 셀<sup>cell</sup>을 생성하는 태그, tr 내부에서 사용 | `rowspan`, `colspan` |
 | `td` | 표의 데이터 셀<sup>cell</sup>을 생성하는 태그, tr 내부에서 사용 |  |

 ### **[ 공간 분할 태그 ]**

<br>

- `inline 요소` : 옆으로 나열되는 요소 (a태그, 글자 형태 관련 태그 등), **span 태그**

- `block 요소` : 위에서 아래로 쌓이는 형태로 나열되는 요소 (제목 태그, p 태그 등), **div 태그**

<br>

## **멀티미디어 관련 태그** 
---
<br>

 | 태그 | 설명 | 속성 |
 |---|:---:|---:|
 | `img` | 이미지를 넣기 위해 사용 | src(이미지 주소 지정), alt(이미지 로드 불가 시 나오는 글자 지정), width, height|
 | `audio` | 오디오를 재생하기 위해 사용 | src(음악 파일 경로 지정), preload(재생 전 모두 불러올지 지정), autoplay, loop, controls (음악 재생 도구 출력 여부 지정) |
 | `source` | 지원하는 음악 파일의 종류가 다른 문제를 해결하기 위한 태그 |  |
 | `video` | 동영상을 재생하기 위해 사용 | `audio` 태그와 유사 |

<br>

## **입력 양식 태그** 
---
<br>

- `form 태그` : 입력 양식을 만들기 위한 태그, form 태그 내부에 다양한 입력 태그를 배치하여 양식 작성

- `input 태그` : 사용자로부터 정보를 입력 받는 기능을 수행하는 태그

- `textarea 태그` : 여러 줄의 텍스트를 입력받는 기능을 수행하는 태그

- `select 태그` : 여러 개의 목록에서 몇 가지를 선택할 수 있는 입력 양식 요소

- `label 태그` : input태그와 같은 입력 양식에 대한 설명을 넣기 위해 사용

- `fieldset 태그` : 입력 양식들을 하나의 그룹으로 묶기 위해 사용.

- `legend 태그` : fieldset에 대한 설명을 제공

  > **tip: radio 표기법에서 name으로 구분되기에 같은분류는 이름 같게해줘야함. ( 여러개중 한개만 선택가능)**

<br>

**실습 코드** (form.html 중 일부)

``` html
<body>
  <h2>입력 양식 태그 실습</h2>
  <form>
    <fieldset> <!--하나의 그룹으로 묶음-->
      <legend>기본 정보</legend>
      <label for="email">이메일</label>
      <input id="email" type="email" name="email" placeholder="이메일 입력"><br>

      <label for="password">비밀번호</label>
      <input id="password" type="password" name="password" placeholder="비밀번호 입력"><br>

      <label for="confirm-password">비밀번호 확인</label>
      <input id="confirm-password" type="password" name="confirmPassword"
           placeholder="비밀번호 재입력"><br>
      <label for="birth">생년월일</label>
      <input id="birth" type="date" name="birth" placeholder="생년월일 입력"><br>

      <input id="male" type="radio" name="gender" value="male">
      <label for="male">남</label>
      <input id="female" type="radio" name="gender" value="female">
      <label for="female">여</label><br>
    </fieldset>

    <fieldset> <!--하나의 그룹으로 묶음-->
      <legend>추가 정보</fieldset>

      <label for="hobbies">취미 선택</label><br>
      <select id="hobbies" name="hobby" multiple>
        <option value="html">HTML</option>
        <option value="css">CSS</option>
        <option value="js">JavaScript</option>
        <option value="node">Node.js</option>
        <option value="db">Database</option>
      </select><br>

      <label for="intro">소개글</label><br>
      <textarea id="intro" name="intro"
                cols="50" rows="4" placeholder="200자 이내로 입력"></textarea>
    </fieldset>

    <input type="submit" value="회원가입">
  <!-- button으로 대체도 가능 : <button type="submit">회원가입</button> -->
  </form>
  <a href="./">홈으로 이동</a>
</body>
</html>

```

## **알아두면 좋은 VS CODE 단축키** 
---
<br>

- **[SHIFT] +[DELETE]** : 한줄 다지워짐
- **[CTRL] + [ENTER]** : 바로 다음줄로 넘어감.
- **[CTRL] + [/]** : 주석처리
- **[ALT]+[SHIFT]+[↓]** : 줄 복사
- **[SHIFT]+[ALT]+[F]** : 들여쓰기 정리

## **표기법** 
---
<br>

- **confirm-password 케밥 표기법** : 보통 css에서 사용
- **confirmPassword 카멜 표기법** : 자바, 자바스크립트같은 프로그래밍언어에서 변수명 사용할 때 사용
- **confirm_password 스네이크 표기법** : C, Python
