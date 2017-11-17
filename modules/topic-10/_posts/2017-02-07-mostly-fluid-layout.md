---
title: Mostly Fluid Layout
module: 10
---

# The Mostly Fluid Layout

<div class="embed-responsive embed-responsive-16by9"><iframe class="embed-responsive-item" src="https://www.youtube.com/embed/Eh9R2nppvNY" frameborder="0" allowfullscreen></iframe></div>

<div id="code-heading">HTML</div>

```html
<div class="container">
    <div class="box dark_blue"></div>
    <div class="box light_blue"></div>
    <div class="box green"></div>
    <div class="box red"></div>
    <div class="box orange"></div>
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
    height: 100px;
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
.red {
    background-color: #a40000;
}
.orange {
    background-color: #dd8400;
}

@media (min-width: 450px) {
    .light_blue, .green {
        width: 50%;
    }
}

@media (min-width: 550px) {
    .dark_blue, .light_blue {
        width: 50%;
    }
    .green, .red, .orange {
        width: 33.33333%;
    }
}

@media (min-width: 700px) {
    .container {
        width: 700px;
        margin-left: auto;
        margin-right: auto;
    }
}
```

<div class="displayed_code_example">
    <div class="embed-responsive" style="padding-bottom:500px"><iframe class="embed-responsive-item" src="https://montana-media-arts.github.io/341-work/lectureCode/10/mostly-fluid-01/" frameborder="0" allowfullscreen></iframe></div>
</div>

| [**[Code Download]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/10/mostly-fluid-01/mostly-fluid-01.zip) | [**[View on GitHub]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/10/mostly-fluid-01/) | [**[Live Example]**](https://montana-media-arts.github.io/341-work/lectureCode/10/mostly-fluid-01/) |
