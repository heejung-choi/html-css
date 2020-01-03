# 20200103 html_test day21

## 문자 입력 연습

```html
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Insert title here</title>
</head>
<body>
<h1>오늘은 그냥 금요일..</h1>
<h2>오늘은 그냥 금요일..</h2>
<h3>오늘은 그냥 금요일..</h3>
<h4>오늘은 그냥 금요일.</h4>
<h5>오늘은 그냥 금요일.</h5>
<h6>오늘은 그냥 금요일</h6>>

</body>
</html>
```



## 문자, 이미지, 테이블 입력 연습

```html
<!DOCTYPE html>
<html>
<head><!--이런저런정보-->
<meta charset="UTF-8">
<title>HTML 학습</title>
</head>
<body>
<h1>자주 사용되는 HTM 태그 학습</h1>
<hr> <!--<hr> 분리선을 그려준다-->
<h2>하이퍼링크 태그</h2>
<a href="http://www.w3.org/"> w3 컨소시엄</a><br>
<a href="http://www.w3schools.com">Web client 기술 학습 사이트</a><br>
<a href="http:java.sun.com"><img src="../images/abc.jpg"></a>
<img src="https://newsimg.sedaily.com/2019/12/04/1VRXYSKJF8_4.jpg">
<h2>이미지 출력 태그</h2>
<img src="../images/duke_luau.png"width="100"><!--상대 URL  -->
<img src="/edu/images/duke_luau.png"width="100" height="300"><!--상대 URL  -->
<img src="http://localhost:8000/edu/images/duke_luau.png"><!--절대 URL  -->
<!--<br> 행바꿈을 해주는 태그  -->
<!--하이퍼링크를 사용하고 싶을 때 <a>를 사용한다.  -->
<h2>리스트 태그</h2>
<UL> <!-- 동그라미 글머리 기호 -->
	<li>Java programming</li>
	<li>SQL</li>
	<li>HTML5</li>
	<li>CSS3</li>
	<li>JavaScript</li>
	<li>Ajax</li>
	<li>servlet</li>
	<li>JSP</li>
	<li>JDBC</li>
</UL>
<hr>
<ol> <!-- 숫자기호 -->
	<li>Java programming</li>
	<li>SQL</li>
	<li>HTML5</li>
	<li>CSS3</li>
	<li>JavaScript</li>
	<li>Ajax</li>
	<li>servlet</li>
	<li>JSP</li>
	<li>JDBC</li>
</ol>
<h2>테이블 태그</h2>
<table border="1"> <!-- border 테이블에 선을 그려지게 한다.  -->
	<tr><th>언어이름</th><th>설명</th></tr><!-- 제목행 -->
	<tr><td>Java</td><td>범용으로 활용되는 oop언어</td></tr><!--실제 컨텐트행 -->
	<tr><td>JavaScript</td><td>동적인 웹페이지 개발에 사용하는 oop언어</td></tr>
	<tr><td>CSS</td><td>HTML의 스타일을 조정하는 언어</td></tr>
	<tr><td>R</td><td>통계분석과 데이터 마이닝에 사용되는 언어</td></tr>
	<!-- <th> 고딕체 가운데 정렬 , <td> 왼쪽 정렬 -->
</table>
<h2>입력 폼 태그</h2>
<form action="..."method="">
	<input type="text" placeholder="이름을 입력하세요..." required name="gname">
	<br>
	<input type="number" placeholder="나이를 입력하세요..." required name="gage">
	<br>									
	<input type="date" name="gdate"><label>원하는 날짜를 입력하세요...</label>
	<br>
	성별을 선택하세요:<br>
	남성 <input type="radio" name="gender" value= "male">								
	여성  <input type="radio" name="gender" value = "female">
	<br>
	좋아하는 음식을 선택하세요:<br>
	떡볶이 <input type="checkbox" name="food"value= "떡볶이 ">								
	피자 <input type="checkbox" name="food"value= "피자">	
	파스타 <input type="checkbox" name="food"value= "파스타">	
	한우 <input type="checkbox" name="food"value= "한우">	
	라면 <input type="checkbox" name="food"value= "라면">	
	<br>														
<input type="submit" value="전송">
</form>
<!--  -->
</body>
</html>

```



## HTML mark

```html
<!DOCTYPE html>
<html>
<body>

<p>Do not forget to buy <mark>for get buy 밀크우유</mark> today. <mark>for get buy 밀크우유</mark> today.  <mark>for get buy 밀크우유</mark> today. <mark>for get buy 밀크우유</mark> today.</p> 

<p>Do not forget to buy <mark>for get buy 밀크우유</mark> today.</p>
<p>Do not forget to buy <mark>for get buy 밀크우유</mark> today.</p>

<p><strong>Note:</strong> The mark tag is not supported in Internet Explorer 8 and earlier versions.</p>

</body>
</html>

```



## HTML p tag 

```htmlhtml
<!DOCTYPE html>
<html>
<body>

<p>This is a paragraph.</p>
<p>This is a paragraph.</p>
<p>This is a paragraph.</p>

<hr>

This is a paragraph.<br>
This is a paragraph.<br>
This is a paragraph.<br>

</body>
</html>
```

## HTML picture Tag

```html
<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>
<!-- 반응형 웹 -->
<!--화면 사이즈에 따라 입력할 수 이미지를 다르게 나타낸다.  -->
<picture>
  <source media="(min-width: 650px)" srcset="img_pink_flowers.jpg">
  <
  
  <source media="(min-width: 465px)" srcset="img_white_flower.jpg">
  <img src="img_orange_flowers.jpg" alt="Flowers" style="width:auto;">
</picture>

<p>Resize the browser to see different versions of the picture loading at different viewport sizes.
The browser looks for the first source element where the media query matches the user's current viewport width,
and fetches the image specified in the srcset attribute.</p>

<p>The img element is required as the last child tag of the picture declaration block.
The img element is used to provide backward compatibility for browsers that do not support the picture element, or if none of the source tags matched.
</p>

<p><strong>Note:</strong> The picture element is not supported in IE12 and earlier or Safari 9.0 and earlier.</p>

</body>
</html>

```

## HTML figure Tag

```html
<!DOCTYPE html>
<html>
<body>

<p>The Pulpit Rock is a massive cliff 604 metres (1982 feet) above Lysefjorden, opposite the Kjerag plateau, in Forsand, Ryfylke, Norway. The top of the cliff is approximately 25 by 25 metres (82 by 82 feet) square and almost flat, and is a famous tourist attraction in Norway.</p>
<!--이미지를 출력하면서 이미지에 제목을 붙이고 싶을때 사용한다. HTML5 부터 지원되는 기능-->

<figure>
  <img src="img_pulpit.jpg" alt="The Pulpit Rock" width="304" height="228">
</figure>
<p><strong>Note:</strong> The figure tag is not supported in Internet Explorer 8 and earlier versions.</p>

</body>
</html>

```



## HTML textarea Tag

```html
<!DOCTYPE html>
<html>
<body>

<!--방명록에 입력하고 싶을 때 큰 입력상자를 넣고 싶으면 이것을 사용한다.-->

<textarea rows="4" cols="50"> <!-- 4행 50열 -->
At w3schools.com you will learn how to make a website. We offer free tutorials in all web development technologies.
</textarea>

<br>
<!-- row 행의 갯수 cols 넓이 -->
<textarea rows="4" cols="20">
row 행의 갯수
cols 넓이
</textarea>


</body>
</html>

```

## HTML select Tag

```html
<!DOCTYPE html>
<html>
<body>

<!--<select> 하나만 쓸 수 있는 기능(radio와 비슷)/ multiful을 사용하면 여러개를 사용할 수 있다. -->

<select>
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="opel">Opel</option>
  <option value="audi">Audi</option>
</select>
  
</body>
</html>

```

