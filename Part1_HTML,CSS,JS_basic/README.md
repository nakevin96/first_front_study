<span style="color:black;background-color: #F2FE8A; font-size:180%"> **👁‍🗨HTML이란?**</span>  

HTML은 **Hypertext Markup Language**의 약자로  
웹 브라우저 상에서 보여지도록 디자인 된 문서를 말한다.  
  
```html
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8>
        <meta name="viewport" content="width=device-width">
        <title>HELLO</title>
    </head>
    <body>

    </body>
</html>
```
위 코드를 이용하여 가장 기본적인 html구조에 대해 알아보자  
</br>
`!DOCTYPE`이란 <u>_document type이 html이다_</u> 라고 정의하는 것이다.  
</br>
`!DOCTYPE`다음에는 바로 `<html>`이 나오는 것을 확인할 수 있으며 이는 제일 상위에 존재하는 태그이다.  
`<html>`내부에는 `<head>`태그와 `<body>`태그가 위치하게 된다.  
일반적으로 `<head>`에는 사용자에게 보여지는 UI적요소가 존재하지 않으며  
'타이틀', '부가설명', '제목', '아이콘', 'css연결'등의 meta data가 속한다.  
`<meta charset='utf-8'>`이라는 것은 8bit unicode transformation format이라는 뜻으로, 이 페이지의 글자의 포맷이 utf-8을 따른다는 의미이다. 현존하는 대부분의 언어를 지원하기 때문에 기본으로 많이 사용한다.  
그 다음 `<meta name="viewport" content="width=device-width">`는 디바이스 전체 넓이를 사용한다는 의미이다.  
마지막으로 `<title>`은 브라우저를 띄웠을 때 나오는 탭 제목이다.
</br>  

`<body>`가 바로 사용자에게 보여지는 최상위 컨테이너로, 이 안에 작성하는 코드들이 유저들에게 보여진다.
</br>
</br></br></br>
<span style="color:black;background-color: #F2FE8A; font-size:180%"> **👁‍🗨TAG란?**</span>  
  
  이사를 할 때 어느 물건이 어느 방의 물건인지, 그리고 방 안의 물건에서도 어느 위치에 있던 물건인지에 따라 나누어 담은 후 이사를 한다.  
  위와 같이 이사를 하면 짐을 푼 후 제자리에 정리하기도 편해진다.  
  </br>
  태그도 이와 마찬가지로 **박스**의 역할을 하는 태그와, **물건**의 역할을 하는 태그가 존재한다.  
  사용자에게 보여지는 '물건'의 역할과 페이지의 섹션을 나누는 태그들이 존재하는 것이다.  
  </br>
  <img src="https://wikidocs.net/images/page/86842/semantic2.PNG" width="450">  
    
가장 상단은 `<header>` 그 밑은 네비게이션 바인 `<nav>`, 사이드 바인 `<aside>`  
메인 컨텐츠인 `<section>`, 세부 컨텐츠인 `<article>`, 가장 하단 정보인 `<footer>`로 기본 구조를 생각할 수 있다.  
</br>
사용자에게 보여지는 '물건'의 개념인 태그들도,  
**BLOCK**과 **INLINE**으로 나눌 수 있다.  
</br>
Block 레벨이라면 한 줄을 전부 차지하기 때문에 충분한 공간이 있더라도  
바로 다음에 오는 아이템이 다음 라인에 나오게 되고,  
Inline 레벨일 때는 충분한 공간이 있을 때 연달아 나오는 아이템이 한 줄에 같이 구현된다.  
<img src="https://i.stack.imgur.com/UCxMx.png" width="450">  
태그라는 것은 <>로 시작하고 </>로 끝나며  
태그 안에 존재하는 내용을 element, 태그를 포함한 전체를 Element, 혹은 node라고 부른다.  
tag의 종류에 대한 코드는 tag_prac.html을 보도록 하자.  
</br></br></br>
<span style="color:black;background-color: #F2FE8A; font-size:180%"> **👁‍🗨CSS란?**</span>  
  
CSS는 **Cascading Style Sheet**의 약자로 HTML을 꾸며주는 역할을 한다.  
스타일을 정리한 문서인데 여기서 'Cascading'이란 '폭포처럼 쏟아지는 물'과 같이 위에서 아래로 떨어지는 형태를 의미한다.  
스타일링을 작성한 문서, 브라우저에서 기본적으로 제공하는 UI 스타일링 등 다양한 스타일링 정의가 있을 때,  
특정 요소에대한 스타일의 세부적인 정의가 있다면 사용하고, 없다면 다음 스타일링을 확인하며 특정 요소의 스타일을 지정한다.  
</br>
웹사이트를 스타일링 할 때, 간단하게만 스타일의 종류를 나누어본다면 **개발자가 작성하는 style sheet**(css파일- Author style), 브라우저 상에서 다크모드와 같이 **사용자의 취향에 맞게 변경되는 스타일**(User style), **브라우저에 기본적으로 지정되어 있는 스타일** (Browser style)로 나눌 수 있다.  
여기서의 Cascading을 한 번 생각해보면,  
만약 브라우저가 버튼을 화면에 구현하려고 하는데, Author style이 있다면 해당 스타일을 사용하고 없다면 User Style을 확인하여 정의한다. 만약 사용자가 지정한 스타일링도 존재하지 않는다면 그 때 브라우저의 기본 스타일을 이용해 버튼을 구현한다.  
이렇게 Author style -> User style -> Browser style로 확인을 진행하는 과정을 **Cascading**이라 하는 것이다.  
</br>
Cascading의 연결고리를 끊어내는 `!important`라는 문법이 있기는 한데, 이는 별로 좋지 못한 방법이니, html의 구조를 수정하던가 css의 구조를 수정하는 것이 좋다. 
</br></br></br>
<span style="color:black;background-color: #F2FE8A; font-size:180%"> **👁‍🗨CSS의 Selector는 무엇일까?**</span>  
</br>
<img src="https://velog.velcdn.com/images%2Frameau17%2Fpost%2F9fa8ba78-b8e7-41d4-9f96-157c5b8309a1%2F2z4a3yh4.jpeg" width="450"> 
  
Selector(선택자)라는 것은 HTML의 어떤 태그들을 고를 것인지 규정하는 문법이다.  
`*`은 모든 태그  
`tag name`은 특정 이름을 갖는 태그  
`#id`는 해당하는 id를 갖는 태그  
`.class`는 해당하는 클래스를 갖는 태그  
`:`는 State를 달 수 있는 문법  
`[]`는 속성값 attribute만 골라서 적용하는 문법을 말한다.  
```css
selector {
  property: value;
}
```  
위와 같이 selector로 적용하고자 하는 태그부분을 지정하고 property와 value를 이용해 스타일을 꾸미게 된다.  
자세한 적용은 `css_prac.html`을 보자.  
