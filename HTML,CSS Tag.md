# HTML Tag /CSS Tag

# html

```HTML
<head>
<!--이런저런정보-->
    
<br> 
<!--행바꿈을 해주는 태그  -->
    
<p></p>
<!--하나의 문단을 만들 때 쓰임-->
    
<a></a>
<!--하이퍼링크를 사용하고 싶을 때 사용한다.  -->

    
<img>
<img src="my_profile.png" width="500" height="300">
<!-- 이미지를 삽입하는 태그, src 속성을 통해 이미지 경로를 지정한다.-->
    
<hr>
<!-- 분리선을 그려준다-->
    
<UL> 
<!-- 동그라미 글머리 기호 --> 
    
<ol>
<!-- 숫자기호 -->
    
<th colspan="3">
<!-- 열병합 -->
<td rowspan="2"> 
<!-- 행병합 --> 
    
<li>
<!-- 태그는 list의 약자로, 목록을 만드는 태그-->
    
&lt;개행&gt;
<!-- 문자에 괄호를 쓸 때 [] ()는 써도 괜찮지만, 꺽세괄호를 만나면 태크로 인식하기 때문에 일반 문자에 <>는 쓰면 안된다.
꺽세괄호를 쓰고 싶을때  &lt;개행&gt;를 사용해야 한다.-->

&nbsp;
<!-- 블랭크를 많이 쓰고 싶을 때 하나의 공백을 의미하는 &nbsp;을 사용하면 된다. &nbsp; 한개당 하나의 블랭크로 인식한다.-->
 
<br>
<!-- br태그는 닫는 괄호가 없다는 인식이 있을 수 있게<br/> 이렇게 작성하는 방식과<br> 이렇게 작성하는 방식이 있다.  -->

<fieldset> 하나의 박스로 묶는다는 것    
    
전화번호의 정규표현식   
<label for=phone>연락처</label>
<input id=phone name=phone type=tel 
placeholder="00*-000*-0000" 
pattern="[0-9]{2,3}-[0-9]{3,4}-[0-9]{4}"
<!-- pattern안에 '-' 기호를 반드시 넣어야 한다. --> 
    
생일 최댓값 최솟값 설정
<label for=date_of_birth>생일</label>
		<input id=date_of_birth name=date_of_birth type=date min="1950-01-01" max="2000-01-01">
<!--  min과 max를 통해 최솟값과 최댓값을 설정할 수 있다. -->

홈페이지 주소 설정
<label for=homepage>홈페이지</label>
		<input id=homepage name=homepage type=url>


option 을 통해 추천 리스트 설정
<label for=favorite_star>좋아하는 연예인</label>
		<input id=favorite_star name=favorite_star type=text list=favorite_star_list>
		<datalist id=favorite_star_list>
			<option value=윤아>
			<option value=태연>
			<option value=유리>
			<option value=제시카>	
			<!-- option: 추천 리스트 -->
        </datalist>
 
```



# css

```html
- color 정하기
	<h2 style ="color:red; background-color: yellow">도우너</h2>
	<h2 style ="color:red; background-color: yellow">도우너</h2>


- 선택하면 빨간색으로 변경: hover
	<style>
	#t1:hover{
		font-weight : bold;
		color :red;
	}
	</style>


- 투명하게: opacity
	<style>
	.t2:hover {
	opacity :0.3;
	<!-- 0.0(완전 투명)~1.0(완전 불투명) -->
	}
	</style>

- 테두리선: border
	border : 1px solid blue; //실선
	border : 1px dotted red; //점선
	border-radius : 5px;//모서리 부분 둥글게




- 특정 부분만 다르게 적용하고 싶다면 
	:<div></div>, <span></span>

css를 다르게 적용하려는 태그 또는 태그의 컨텐트에 정의하는 용도의 태그들
	<div>:행바꿈 해서 변경 (여러 태그들을 묶거나 또는 태그에 대하여 CSS 	속성을 적용할 때)
	<span>: 행바꿈 하지 않고 변경 (컨텐트의 일부분에 대하여 CSS속성을 적	용할 때)

    
    
- 공통의 이름 class
	.sampleclass {text-decoration:underline;}


- 싱글 이름 id
	#sampleid {text-decoration: underline;
	}
	#t1:hover{
		font-weight : bold;
		color :red;
	}
	<!--hover 마우스를 가져다 놓으면 그것만 빨간색으로 변한다. -->




```



