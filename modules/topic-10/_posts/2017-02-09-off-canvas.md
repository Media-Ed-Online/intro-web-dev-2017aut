---
title: Off Canvas
module: 10
---

# Off Canvas

The following example demonstrates the "off canvas" menu that is common in mobile designs. There is _some_ javascript in this example. If you find yourself wanting to use this design pattern in a future site, just copy the javascript in. You will learn about javascript in another class.

<div class="embed-responsive embed-responsive-16by9"><iframe class="embed-responsive-item" src="https://www.youtube.com/embed/tZkyUL22qQA" frameborder="0" allowfullscreen></iframe></div>

<div id="code-heading">HTML</div>

```html
<nav id="drawer" class="dark_blue">
  <h2>Off Canvas</h2>
  <p>Click outside the drawer to close</p>
</nav>

<main class="light_blue">
  <a id="menu">
    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
      <path d="M2 6h20v3H2zm0 5h20v3H2zm0 5h20v3H2z"/>
    </svg>
  </a>
  <p>Click on the menu icon (hamburger icon) to open the drawer</p>
</main>

<script>
  /*
   * Open the drawer when the menu is on is clicked.
   */
  var menu = document.querySelector('#menu');
  var main = document.querySelector('main');
  var drawer = document.querySelector('#drawer');

  menu.addEventListener('click', function(e) {
    drawer.classList.toggle('open');
    e.stopPropagation();
  });
  main.addEventListener('click', function() {
    drawer.classList.remove('open');
  });

</script>
```


<div id="code-ruler"></div>
<div id="code-heading">CSS</div>

```css
@import url(https://fonts.googleapis.com/css?family=Roboto);

html, body {
  margin: 0;
  padding: 0;
}

body {
  font-family: 'Roboto', sans-serif;
}


.box {
  min-height: 150px;
}

.dark_blue {
  background-color: #2A457A;
  color: #efefef;
}

.light_blue {
  background-color: #099DD9;
}


html, body {
  height: 100%;
  width: 100%;
}
a#menu svg {
  width: 40px;
  fill: #000;
}
nav, main {
  padding: 1em;
  box-sizing: border-box;
}
main {
  width: 100%;
  height: 100%;
}


/*
 * Off-canvas layout styles.
 */

/* Since we're mobile-first, by default, the drawer is hidden. */
nav {
  width: 300px;
  height: 100%;
  position: absolute;
  /* This trasform moves the drawer off canvas. */
  -webkit-transform: translate(-300px, 0);
  transform: translate(-300px, 0);
  /* Optionally, we animate the drawer. */
  transition: transform 0.3s ease;
}
nav.open {
  -webkit-transform: translate(0, 0);
  transform: translate(0, 0);
}

/* If there is enough space (> 600px), we keep the drawer open all the time. */
@media (min-width: 600px) {

  /* We open the drawer. */
  nav {
    position:relative;
    -webkit-transform: translate(0, 0);
    transform: translate(0, 0);
  }

  /* We use Flexbox on the parent. */
  body {
    display: -webkit-flex;
    display: flex;
    -webkit-flex-flow: row nowrap;
    flex-flow: row nowrap;
  }

  main {
    width: auto;
    /* Flex-grow streches the main content to fill all available space. */
    flex-grow: 1;
  }
}

/* If there is space (> 800px), we keep the drawer open by default. */
@media (min-width: 600px) {
  main > #menu:after {
    content: 'The drawer stays open if width > 600px';
  }
  main p, nav p {
    text-decoration: line-through;
  }
}
```

<div class="displayed_code_example">
    <div class="embed-responsive" style="padding-bottom:500px"><iframe class="embed-responsive-item" src="https://montana-media-arts.github.io/341-work/lectureCode/10/off-canvas-01/" frameborder="0" allowfullscreen></iframe></div>
</div>

| [**[Code Download]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/10/off-canvas-01/off-canvas-01.zip) | [**[View on GitHub]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/10/off-canvas-01/) | [**[Live Example]**](https://montana-media-arts.github.io/341-work/lectureCode/10/off-canvas-01/) |
