```
Table
```

#  TABLE

<TR> 행을 만듬</TR>

<TH> (TD업그레이드)상단의 제목</TH>

<TD>행에 들어가는 내용</TD>

  border: 1px solid black  테이블에 두선의 박스를 만든다

 border-collapse: collapse; 위와 같이 써주면 선이 하나인 이쁜 테이블이 완성된다 (깔끔)

<colgroup>은 표의 열을 묶는다.

 <colgroup>

  <col span="2" style="background-color:red"> 2개의 열을 묶어서 바탕을 빨간색으로 칠한다

  <col style="background-color:yellow">한개의 바탕을 노란색으로 칠한다

 </colgroup>



####  Cell Padding  표의 셀 내부의 패딩과 셀 사이의 공간을 조정할수 있다

 padding-top: 10px;
 padding-bottom: 20px;
 padding-left: 30px;
 padding-right: 40px;

또는 padding 50px 45px 30xp 15px  //(위 오른쪽 아래 왼쪽 시계방향대로 적어도 된다);



######  border-spacing 테두리 간격 설정

안이쁘다...

\table {
 border-collapse: separate;
 border-spacing: 15px;
}

##   **colspan,** **rowspan**  중요!



### **colspan**

하나의 셀 또는 행을 여러 열로 나누고 둘 이상의 열로 합병하기 위해서 사용

 <!DOCTYPE html>

<html>

 

<head>

<style>

table, th, td {

  border: 1px solid black;

  border-collapse: collapse;

}

th, td {

  padding: 5px;

  text-align: left;   

}

</style>

</head>

 

<body>

 

<h2>Cell that spans two columns:</h2>

<table style="width:100%">

 <tr>

  <th>Name</th>

  <th colspan="2">Telephone</th>

 </tr>

 <tr>

  <td>Bill Gates</td>

  <td>555 77 854</td>

  <td>555 77 855</td>

 </tr>

</table>

 

</body>

</html>

###  **rowspan** 

하나의 셀을 두개 이상으로 확장하거나 셀을 여러 행으로 나눌 때 사용

<!DOCTYPE html>

<html>

 

<head>

<style>

table, th, td {

  border: 1px solid black;

  border-collapse: collapse;

}

th, td {

  padding: 5px;

  text-align: left;   

}

</style>

</head>

 

<body>

 

<h2>Cell that spans two rows:</h2>

<table style="width:100%">

 <tr>

  <th>Name:</th>

  <td>Bill Gates</td>

 </tr>

 <tr>

  <th rowspan="2">Telephone:</th>

  <td>555 77 854</td>

 </tr>

 <tr>

  <td>555 77 855</td>

 </tr>

</table>

 

</body>

</html>

##  colspan 헤더셀과 데이터셀이 가로로 합병하여 테이블이 이상해질 일이 없지만 rowspan 경우에는 헤더셀을 건드릴 경우 테이블이 이상해지고 셀은 세로로 합병됩니다.

0
