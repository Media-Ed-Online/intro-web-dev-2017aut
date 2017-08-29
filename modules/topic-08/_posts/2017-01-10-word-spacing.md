---
title: Word Spacing
module: 9
---

# Word Spacing

In addition to being able to adjust the space between characters, developers can adjust the amount of space between words only, using the `word-spacing: ` property.

<div id="code-heading">CSS</div>

```css
.example-container h2 {
    font-family: "Helvetica", sans-serif;
    line-height: 1.5em;
    font-weight: 100;
    margin-bottom: 2em;
    text-align: center;
}

h2.no-space {
    word-spacing: normal;
}

h2.some-space {
    word-spacing: 0.8em;
}

h2.lots-space {
    word-spacing: 3em;
}

h2.negative-space {
    word-spacing: -0.8em;
}
```

<div id="code-ruler"></div>
<div id="code-heading">HTML</div>

```html
<div class="example-container">
    <h2 class="no-space">No Space Applied</h2>
    <h2 class="some-space">Some Space Applied</h2>
    <h2 class="lots-space">A Lot of Space Applied</h2>
    <h2 class="negative-space">Negative Space Applied</h2>
</div>
```

<div class="displayed_code_example">
<style>
    .example-container h2 {
        font-family: "Helvetica", sans-serif;
        font-size: 1.2em;
        line-height: 1.5em;
        font-weight: 100;
        margin-bottom: 2em;
        text-align: center;
    }

    h2.no-space {
        word-spacing: normal;
    }

    h2.some-space {
        word-spacing: 0.8em;
    }

    h2.lots-space {
        word-spacing: 3em;
    }

    h2.negative-space {
        word-spacing: -0.8em;
    }
    </style>
    <div class="example-container">
        <h2 class="no-space">No Space Applied</h2>
        <h2 class="some-space">Some Space Applied</h2>
        <h2 class="lots-space">A Lot of Space Applied</h2>
        <h2 class="negative-space">Negative Space Applied</h2>
    </div>
</div>

| [**[View on GitHub Download]**](https://github.com/Montana-Media-Arts/341-work/tree/master/lectureCode/08/word-spacing-01/index.html) | [**[Live Example]**](https://montana-media-arts.github.io/341-work/lectureCode/08/word-spacing-01/) |
