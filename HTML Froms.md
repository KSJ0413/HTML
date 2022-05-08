#  HTML Froms....... list

## Forms

​      **사용자로부터 데이터를 받아야 하는 경우 사용되는 요소들을 폼 요소라고 한다**

 **폼 요소는 서버에 데이터를 전달하기 위한 요소이며, <input> 은 대표적인 폼 요소이다.** 

**<input>은 내용이 없고, type을 통해 입력 양식을 나타낸다**





#  매우 중요하다!!!!

##  Text, Password

 주로 아이디,이름, 주소등 단순한 텍스트를 입력 시에 Text를 사용한다.

​    Password의 경우에는  값이 노출되지 않아야 하는 경우 주로 사용한다.

ID : <input class = 'id' type="text" placeholder="아이디를 입력해주시기 바랍니다."><br> PW : <input type="password">





 \- action 속성 : 사용자가 입력한 값을 server-side script로  보내서 받을 수 있는 webpage 요청
 \- method 속성 : 사용자가 입력한 값을 Server-Side Script로 보낼때 HTTP Method를 설명한다
       (GET or POST)
  GET  - 민감한 정보를 보내지 않고 페이지 요청시 사용함, 주소에 서브밋되는 정보가
      노출됨, 검색할 때 사용
  POST- 민감한 정보를 보내면서 페이지 요청시 사용함, 주소에 서브밋되는 정보가
      노출되지 않음. 서버에 자원 생성을 위해 사용

<form action="action_page.jsp" **method=****"GET"**>  이 경우 말고도 GET 방식의 페이지
                                   요청은 많음

 <form action="action_page.jsp" **method=****"POST"**> 이 경우만 POST 방식의 페이지를 요청함



* **textarea** : 한줄만 입력하는 text와 달리 여러줄 입력할떄 이용한다
* **button**:  (**submit, reset, button**) 3개의 버튼타입을 나타낼수있다 
* **select**: 항목의 값을 지정할수있다
* **label**: Form 태그 요소를 연결시켜줄떄 사용한다.
* **fieldset**: 요소의 제목으로 활용된다
* **legend**: 폼 요드를을 그룹화 하여 구조적으로 만들때 사용된다.

<fieldset>  

<legend></legend> 

</fieldset>

* **form**: 폼 데이터를 그룹화하여 서버에 전송;
* **action **: 서버 주소;
* **method **:전송방식 지정;(위에 나와 있듯이 GET, POST)



_END_
