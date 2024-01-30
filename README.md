## 'protype-01'

<br>

### • 배포 주소: [https://prototype-kpop.netlify.app/](https://prototype-kpop.netlify.app/)

<br>

#### - 작업 기간: 2021.07

#### - 리팩토링: 2024.01

<br>

### 기술 스택

Development

<p>
<img src="https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=HTML5&logoColor=white" />
<img src="https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=CSS3&logoColor=white" />
</p>

Config

<p>
<img src="https://img.shields.io/badge/npm-CB3837?style=flat&logo=npm&logoColor=white"/></a>
</p>

Environment

<p>
<img src="https://img.shields.io/badge/Visual Studio Code-007ACC?style=flat&logo=Visual Studio Code&logoColor=white"/></a>
<img src="https://img.shields.io/badge/Git-F05032?style=flat&logo=Git&logoColor=white"/></a>
<img src="https://img.shields.io/badge/GitHub-181717?style=flat&logo=GitHub&logoColor=white"/></a>
</p>
<br>

### 전체 페이지

<img src="https://github.com/azure0929/prototype-01/assets/128226527/00de26e5-a359-4404-b8d7-99b6a7a95209" />

<br><br>

### 💻 주요 기능

---

- grid, featherlight cdn

```html
<section class="gallery">
  <div class="focus">
    <a href="html/blog-post-sub-01.html" data-featherlight="iframe"
      ><img src="images/album-01.jpg" alt="love wins all"
    /></a>
    <span>아이유-Love wins all</span>
    <i class="fa fa-plus-circle"></i>
  </div>
</section>
```

```css
.gallery {
  display: grid;
  grid-template-columns: repeat(6, 1fr);
  grid-gap: 10px;
}
.gallery div {
  border-radius: 20px;
  box-shadow: 0 0 30px rgba(0, 0, 0, 0.185);
  overflow: hidden;
  position: relative;
}
.gallery div:before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.5);
  opacity: 0;
  transition: 0.5s;
  pointer-events: none;
}
.gallery div:hover:before {
  opacity: 1;
}
.gallery .focus {
  grid-column: span 2;
  grid-row: span 2;
}
.gallery div a img {
  width: 100%;
  display: block;
}
.gallery div .fa {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%) scale(0.5);
  color: #fff;
  font-size: 30px;
  opacity: 0;
  transition: 0.35;
  pointer-events: none;
}
.gallery div:hover .fa {
  opacity: 1;
  transform: translate(-50%, -50%) scale(1);
}
.gallery div span {
  position: absolute;
  bottom: -50px;
  width: 100%;
  text-align: center;
  padding: 20px;
  font-weight: 500;
  transition: 0.35s;
  color: #fff;
}
.gallery div:hover span {
  bottom: 0;
}

/* Featherlight Custom CSS */
.featherlight .featherlight-content {
  width: 100%;
  height: 100%;
  margin-left: 0;
  margin-right: 0;
  max-height: 100%;
}
.featherlight-inner {
  width: 100%;
  height: 100%;
}
.featherlight .featherlight-close-icon {
  top: 60px;
  right: 60px;
  width: 30px;
  height: 30px;
  background: rgba(11, 35, 112, 0.8);
  color: #fff;
  border-radius: 50%;
  padding: 5px;
  line-height: 1em;
  font-size: 14px;
  box-shadow: 2px 2px 10px rgba(0, 0, 0, 0.6);
  transition: 0.5s;
}
.featherlight .featherlight-close-icon:active {
  box-shadow: rgba(0, 0, 0, 0.2);
  transform: scale(0.75);
}
```
