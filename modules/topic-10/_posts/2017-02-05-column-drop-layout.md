---
title: Column Drop Layout
module: 10
---

# The Column Drop Layout

<div class="embed-responsive embed-responsive-16by9"><iframe class="embed-responsive-item" src="https://www.youtube.com/embed/YLkOC9Pwitw" frameborder="0" allowfullscreen></iframe></div>

<div id="code-heading">HTML</div>

```html
<div class="container">
    <div class="box dark_blue"></div>
    <div class="box light_blue"></div>
    <div class="box green"></div>
</div>
```


<div id="code-ruler"></div>
<div id="code-heading">CSS</div>

```css
.container {
    display: flex;
    flex-wrap: wrap;
}

.box {
    width: 100%;
    height: 300px;
}

.dark_blue {
    background-color: #131c58;
}
.light_blue {
    background-color: #3760cb;
}
.green {
    background-color: #12a400;
}

@media (min-width: 450px) {
    .dark_blue {
        width: 25%;
    }
    .light_blue {
        width: 75%;
    }
}

@media (min-width: 550px) {
    .dark_blue, .green {
        width: 25%;
    }
    .light_blue {
        width: 50%;
    }
}
```

<div class="displayed_code_example">
    <div class="embed-responsive" style="padding-bottom:300px"><iframe class="embed-responsive-item" src="https://montana-media-arts.github.io/341-work/lectureCode/10/column-drop-01/" frameborder="0" allowfullscreen></iframe></div>
</div>

| [**[Code Download]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/10/column-drop-01/column-drop-01.zip) | [**[View on GitHub]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/10/column-drop-01/) | [**[Live Example]**](https://montana-media-arts.github.io/341-work/lectureCode/10/column-drop-01/) |
