# reset.css

- reset.css는 HTML tag 고유의 style 값들을 '0' 으로 만들어준다.
- 브라우저마다 지원하는 태그의 style 값들이 다르다. reset.css를 사용하면 모든 브라우저에서 일관된 디자인을 제공할 수 있다.

## 사용법

- reset.css를 styles.css파일에 import한다. `@import 'reset.css';`
- HTML 문서에 링크를 생성한다. `<link rel="stylesheet" href="CSS\styles.css">`;

# Google Fonts

- 구글 폰트는 라이선스에서 자유로운 952개의 글꼴 라이브러리이자, CSS와 안드로이드를 통해 글꼴을 편하기 사용할 수 있도록 라이브러리와 API를 둘러보기 위한 상호작용 웹 디렉터리이다.
- 원하는 폰트를 선택해 `customizing`한다. 그 다음 아래와 같이 `@import` 한다.
- 폰트에는 다양한 글씨체 `size`가 있다. 필요한 `size`만 다운받아 빠른 속도로 `@import`하게 한다.

```css
<style>
@import url('https://fonts.googleapis.com/css?family=Montserrat:400,700&display=swap');
body{
    font-family: 'Montserrat', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    /*if Montserrat font exist not you use next font */
}
</style>
```

---

- `opacity` 속성은 불투명함의 정도를 나타낸다.
- 클래스마다 css 파일을 분리하면 유지보수를 쉽게 할 수 있다. 예를 들어 `status-bar`에 `error`가 발생했다면 status-bar 클래스의 css파일을 확인하면 된다.
- `inherit` 속성은 부모 요소의 속성 값을 상속받는다. 아래 `a` 태그는 부모 요소로부터 `color` `#020202`을 상속받는다.

```css
body {
  background-color: white;
  padding: 10px 20px;
  color: #020202;
  font-family: "arsenal", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto,
    Oxygen, Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
}

a {
  color: inherit;
}
```

# box-siziing

```css
* {
  box-sizing: border-box;
}
```

- `box`의 `width`는 30px이다. `padding`을 20px 할당하면 `content`는 10px을 사용할 수 있다. 그래서 padding을 사용하면 `content`범위가 줄어들고 `box` 전체 크기는 50px로 늘어난다. (`height`도 커진다.)
- 이 기본설정을 해결하려면 `box-sizing`을 사용해야 한다. `box-sizing`을 사용하면 `padding`을 사용해도 `box`크기가 변하지 않는다.
- `box` 크기를 예측할 수 있어 기본값으로 사용하는 게 좋다.
  <!--`fixed` 속성은 `width` 값을 `100%`로 설정해야한다. 새로운 레이어에 작성하는것이여서-->

---

- `fixed position` 인 상태에서 가운데 정렬 코드는 아래와 같다.

```css
.chat__write {
  position: fixed;
  margin: 0 auto;
  left: 0px;
  right: 0px;
}
```

- `padding`은 아래 순서로 작성해야 한다.

```css
.chat-screen .chat__messages {
  padding: 0px 20px;
  padding-top: 30px;
}
```

- `.chat__write-column input`는 `input` 태그를 가리킨다.
- `.chat__write-column:nth-child(2)`는 `input`태그를 감싸는 `div` 태그를 가리킨다.

```css
.chat__write-column input {
  width: 100%;
  padding: 10px;
  border: none;
  font-size: 14px;
}

.chat__write-column:nth-child(2) {
  /*input*/
  width: 80%;
}
```

- `icon`에 애니메이션 효과를 적용할려면 `input`태그 뒤에 있어야 한다.

```html
<div class="chat__write-container">
  <input type="text" placeholder="Send Message" class="chat__write" />
  <div class="chat__icon-left chat__icon">
    <i class="far fa-plus-square"></i>
  </div>
  <div class="chat__icon-right chat__icon">
    <span class="chat__write-icon">
      <i class="far fa-grin-wink"></i>
    </span>
    <span class="chat__write-icon">
      <i class="fas fa-hashtag"></i>
    </span>
  </div>
</div>
```

- `display : none;` 대신 `opacity : 0;` 코드를 사용하는 것이 좋다. `opacity` 속성은 애니메이션 효과가 적용되기 때문이다.

```css
.chat__write:focus ~ .chat__icon {
  opacity: 0;
  /*focus ~ .chat__icon 코드는 focus 시 chat_icon을 사라지게 한다.*/
}

.chat__icon {
  font-size: 18px;
  transition: opacity 0.5s ease-in-out;
}
```

- `margin`속성은 `animate` 할 수 없다.
