## 과제
### netflix.com/kr FE 넷플릭스 코리아  클론코딩
-한글화 작업 완 by ksh322 <br>
-영어/한글/일본어(?) 전환 기능 추가예정 <br>
-로그인&회원가입 페이지 2개정도 추가예정 <br>

-demo 페이지 배포 by github.io
<br>

## 팀원 소개
SCIT 48기 A반
서동욱님, 김상호님, 강준석님, 장지웅님

## 프로젝트 소개
넷플릭스 코리아 클론코딩
[데모 시연 페이지](https://bankole2000.github.io/netflix)

## 구성 요소 (기술스택)

A basic warmup exercise. Simple, practice oriented, clone of the Netflix Homepage. 
<br> Built with:

- HTML
- CSS
- Vanilla JS - ES6

## Netflix Clone

Clone of the Netflix website as a light HTML CSS and JS excercise - 


</div>





## Learning Points

- CSS Grid
- Styling Tables
- Tabs with Javascript
- Positioning

## Some cool stuff

Usually, people tend to run to CSS Frameworks to develop and style tabs and switching tabs. But here's a pretty simple, basic way of creating switchable tab content using Vanilla JS:

```javascript
const tabItems = document.querySelectorAll(".tab-item");
const tabContentItems = document.querySelectorAll(".tab-content-item");

// Select tab content
function selectItem(e) {
  removeBorder();
  removeShow();
  // Add border to current tab
  this.classList.add("tab-border");
  // Grab content item from DOM
  const tabContentItem = document.querySelector(`#${this.id}-content`);
  // Add show class
  tabContentItem.classList.add("show");
}
function removeBorder() {
  tabItems.forEach(item => item.classList.remove("tab-border"));
}
function removeShow() {
  tabContentItems.forEach(item => item.classList.remove("show"));
}
// Listen for tab click
tabItems.forEach(item => item.addEventListener("click", selectItem));
```

And for the HTML All you really need is this:

```html
<!-- Content Pretty Long so I'll add later -->
<!-- But this is the basic gist -->
<div class="tab-item">
  <!-- Selectors for the different tab content -->
</div>
<div class="tab-content-item">
  <!-- Content of each tab item -->
</div>
<!-- Simply add more selectors and corresponding 
tab content for each selector -->
```

> Also (Just a thought), You could advance this by adding some animations to the selector borders etc.

# Features in Development

I might add the other pages on the Netflix website if I ever come back to refactor ^-^


## Acknowledgments

- Many thanks to [@bradtraversy](https://github.com/bradtraversy) for his awesome courses - _i will not fail you sensei_
- Thanks to [@torvalds](https://github.com/torvalds) For Making the world a better place

