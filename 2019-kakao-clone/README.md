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

## Friends.html

```html
<li class="friends__friend friend">
  <div class="friend__column">
    <img src="images/avatar.jpg" class="g-avatar friend__avatar" />
    <div class="friend__content">
      <span class="friend__name">
        Arteta
      </span>
      <span class="friend__status">
        <!--this is profile status-->
        hello
      </span>
    </div>
  </div>
  <div class="friend__column">
    <div class="friend__now-listening">
      <span>마음 - 폴킴</span>
      <i class="fas fa-play"></i>
    </div>
  </div>
</li>
```

- 모든 프로필 창은 두 개 컬럼으로 구성된다.

<img src='https://user-images.githubusercontent.com/50260620/71883127-161ca000-3179-11ea-84f4-b89104c59d03.jpg' height="900"/>

## github pages

- new branch `gh-pages`를 생성한다.

- github pages 주소는 아래 형식을 따른다.
- username.github.io/[a name of the project]
- 변경은 `master branch`로 한다.

---

<p>모든 폴더와 파일명은 소문자로 저장한다.</p>
<p>'__'는 부모 자식클래스를 구분하기 위해 사용한다.</p>
<p>'-'는 단어를 구분하기 위해 사용한다.</p>
<a href="https://velog.io/@yesdoing/BEM-Block-Element-Modifier-Quick-start">BEM방법론</a
