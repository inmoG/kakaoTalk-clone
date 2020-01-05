# Kakao-clone HTML Part

## index.html

- status-bar 클래스는 부모 클래스다.
- status-bar\_\_column 클래스는 status-bar의 자식 클래스다.
- status-bar\_\_clock 클래스는 status-bar\_\_column의 자식 클래스다.
- 아이콘은 <a href='https://fontawesome.com/'>Font Awesome</a>의 무료 아이콘을 사용한다.
- 아이콘 크기 설정은 `fa-Nx` 코드를 추가해야 한다.

```html
<span class="header__icon">
  <i class="fas fa-cog fa-3x"></i>
  <!--크기는 2x, 3x, 5x, 7x, 9x가 있다.-->
</span>
```

---

<p>'__'는 부모 자식클래스를 구분하기 위해 사용한다.</p>
<p>'-'는 단어를 구분하기 위해 사용한다.</p>
<a href="https://velog.io/@yesdoing/BEM-Block-Element-Modifier-Quick-start">BEM방법론</a>
