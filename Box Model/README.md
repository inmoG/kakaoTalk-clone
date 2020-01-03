## css는 2가지 파트로 구성된다.

- selector 파트 h1, div Tag
- property 파트 property-name : value;

### css 문법

- 태그
h1 {
    property-name : value;
    property-name : value;
}

- id
#h1 {
    property-name : value;
    property-name : value;
}

- class
.h1 {
    property-name : value;
    property-name : value;
}

- 태그와 class
h1 .name 
{
    property-name : value;
    property-name : value;
}

css는 '.css' 확장자를 사용한다.
css를 별도의 파일로 관리한다면 &lt;head&gt; 태그에 &lt;link rel="stylesheet" href="style.css"&gt; 문법을 적용한다.

엘리먼트는 박스다. 그리고 4개 요소 `contents`, `padding`, `border`, `margin`이 있다.

1. margin : 박스의 `border`에서 바깥쪽으로 있는 간격
2. border : 박스의 경계선
3. padding : 박스의 `border`에서 안쪽으로 있는 간격
4. contents : 내용