# Flex

- `inline-block` 속성을 사용하지 않아도 `inline-block` 속성을 적용시킬 수 있다.
- 부모 박스와 자식 박스를 만든다.
- 플렉스는 자식 박스에 적용하지 않는다. 부모 박스 즉 부모 클래스에 적용한다.
- 부모클래스에 `flex` 속성을 할당하면 자식 클래스들에게도 속성이 적용된다.
- 자식박스의 컨텐츠를 조종하고 싶다면 자식박스에 `flex`를 할당하면 된다.
- 창을 줄이면 창에 맞춰 폭이 조정된다.

## 속성

- justify-content : 수평으로 적용된다. `center`, `space-evenly`, `space-around`, `space-between` 등의 속성이 있다.
- align-items : 수직으로 적용된다. `flex-start`, `flex-end`, `center` 속성 등이 있다.
- flex-direction : `column`, `row`, `row-reverse`, `colume-reverse` 등의 속성이 있다. `column` 속성을 사용하면 `justify-content`는 수직이되고 `align-items`은 수평이 된다. 따라서 가운데에 정렬된다.
- flex-wrap : `wrap`, `nowrap` 속성 등이 있다. `nowrap` 이 `default`이며 `wrap` 속성을 사용하면 창이 줄어들었을 경우 새로운 라인을 생성해 박스를 표현한다.`wrap`은 폭을 유지시켜주지만 `nowrap`은 폭을 유지시키지 않는다.

```html
<a href="http://flexboxfroggy.com/#ko">flexbox game</a>
```
