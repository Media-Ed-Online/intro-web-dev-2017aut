---
title: Layout Shifter
module: 10
---

# Layout Shifter

<div class="embed-responsive embed-responsive-16by9"><iframe class="embed-responsive-item" src="https://www.youtube.com/embed/tZkyUL22qQA" frameborder="0" allowfullscreen></iframe></div>

<div id="code-heading">HTML</div>

```html
<div class="container">
    <div class="box dark_blue"></div>
    <div class="container" id="container2">
        <div class="box light_blue"></div>
        <div class="box green"></div>
    </div>
    <div class="box red"></div>
</div>
```


<div id="code-ruler"></div>
<div id="code-heading">CSS</div>

```css
.container {
    width: 100%;
    display: flex;
    flex-wrap: wrap;
}

.box {
    width: 100%;
    height: 150px;
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

@media (min-width: 500px) {
    .dark_blue {
        width: 50%;
        height: inherit;
    }
    #container2 {
        width: 50%;
    }
}

@media (min-width: 600px) {
    .dark_blue {
        width: 25%;
        order: 1;
    }
    #container2 {
        width: 50%;
    }
    .red {
        width: 25%;
        order: -1;
        height: inherit;
    }
}
```

<div class="displayed_code_example">
    <div class="embed-responsive" style="padding-bottom:500px"><iframe class="embed-responsive-item" src="https://montana-media-arts.github.io/341-work/lectureCode/10/layout-shifter-01/" frameborder="0" allowfullscreen></iframe></div>
</div>

| [**[Code Download]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/10/layout-shifter-01/layout-shifter-01.zip) | [**[View on GitHub]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/10/layout-shifter-01/) | [**[Live Example]**](https://montana-media-arts.github.io/341-work/lectureCode/10/layout-shifter-01/) |


# The "Holy Grail" Layout

The "classic" layout is referred to as the "holy grail" layout. This is similar to the layout presented above.

Please read the following article about this layout. This article also contains an elegant solution to the problem using flexbox, as well as a flex-flow solution for easy responsive design.
[Holy Grail Layout](https://philipwalton.github.io/solved-by-flexbox/demos/holy-grail/)
