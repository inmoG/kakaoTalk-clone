# Flex

`inline-block` 속성을 사용하지 않아도 `inline-block` 속성을 적용시킬 수 있다.

플렉스는 부모 클래스에 적용한다.

부모 클래스에 `flex` 속성을 할당하면 자식 클래스에게도 속성이 적용된다.

자식 클래스에 `flex` 속성을 할당하면 클래스 내용에 속성이 적용된다.

창을 줄이면 창에 맞춰 폭이 조정된다.

## 속성

justify-content : 수평(요소 가로 정렬)으로 적용된다. `center`, `flex-end`, `flex-start`, `space-around`, `space-between` 등의 속성이 있다.

align-items : 수직(요소 세로 정렬)으로 적용된다. `flex-start`, `flex-end`, `center` 속성 등이 있다.

flex-direction : `column`, `row`, `row-reverse`, `colume-reverse` 등의 속성이 있다.

flex-wrap : `wrap`, `nowrap` 속성 등이 있다. `nowrap` 이 `default`이며 `wrap` 속성을 사용하면 창이 줄어들었을 경우 새로운 라인을 생성해 박스를 표현한다.`wrap`은 폭을 유지시켜주지만 `nowrap`은 폭을 유지시키지 않는다.

`column-reverse` 또는 `row-reverse`를 사용하면 요소의 `start`와 `end` 방향이 바뀐다.

`Flex`의 방향이 `column`일 경우 `justify-content`의 방향이 세로로, `align-items`의 뱡향이 가로로 바뀐다.

`align-self, order` 는 지정한 요소에만 적용된다.

`align-content`는 여러 줄 사이의 간격을 지정하며, `align-items`는 컨테이너 안에서 모든 요소 정렬 방법을 지정한다.

```css
#pond {
  display: flex;
  justify-content: space-between;
}

.yellow {
  order: -1;
  algin-self: flex-end;
}
```

---

<a href="http://flexboxfroggy.com/#ko">flexbox game</a>
