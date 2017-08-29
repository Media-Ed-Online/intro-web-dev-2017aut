---
title: Psuedo-Classes
module: 8
---

# Psuedo-Classes

In CSS, a "pseudo-class" is an event or state that can be triggered by the browser. When this event is triggered, additional CSS rules can be applied to a page.

The horribly obnoxious ["Conclusions" page from Week-7]({{site.baseurl}}/modules/week-7/conclusions/), utilized CSS pseudo-classes.

This is the same technology that allows browsers to alter the appearance of links when you hover over them, click them, or after you have visited them.

Like pseudo-elements, pseudo-classes are appended after a CSS selector. However note, that pseudo classes are preceded by only a single colon, as opposed to a set.

<div id="code-heading">CSS</div>

```css
/* A CSS Pseudo-Element Selector */
p::first-letter {}

/* A CSS Pseudo-Class Selector */
p:hover {}
```


# Common Pseudo-Classes

NOTE: Any pseudo-class that relies upon mouse information (such as the ones below) will not translate to mobile devices. 

### `:hover`

The `:hover` class is triggered whenever a users mouse "hovers over" the selected element.

<div id="code-heading">CSS</div>

```css
.hover-element {
    font-size: 1em;
    background-color: #545454;
    color: #c4c8c4;
    padding: 1em;
    text-align: right;
}
.hover-element:hover {
    font-size: 4em;
    background-image: url(../imgs/puppy.jpg);
    color: rgb(255, 245, 0);
    text-transform: uppercase;
    font-weight: bold;
    text-align: justify;
    letter-spacing: 0.2em;
    padding: 0em;
    height: 75%;
}
```


<div id="code-ruler"></div>
<div id="code-heading">HTML</div>

```html
<div class="hover-element">
    don't hover over me. please...
</div>
```

<div class="displayed_code_example">
    <style>
    .hover-element {
        font-size: 1em;
        background-color: #545454;
        color: #c4c8c4;
        padding: 1em;
        text-align: right;
    }
    .hover-element:hover {
        font-size: 4em;
        background-image: url(../imgs/puppy.jpg);
        color: rgb(255, 245, 0);
        text-transform: uppercase;
        font-weight: bold;
        text-align: justify;
        letter-spacing: 0.2em;
        padding: 0em;
        height: 75%;
    }
    </style>
    <div class="hover-element">
        don't hover over me. please...
    </div>
</div>

Hover is more often used to specify how link text will appear when a user hovers over it.

<div id="code-heading">CSS</div>

```css
.element-1 {
    font-size: 1.5em;
    font-family: sans-serif;
}
.element-1 a {
    color: #17a200;
    text-decoration: none;
}
.element-1 a:hover {
    color: #ff0000;
    font-style: italic;
}
```


<div id="code-ruler"></div>
<div id="code-heading">HTML</div>

```html
<div class="element-1">
    You should visit the <a href="https://en.wikipedia.org/wiki/The_Garden_of_One_Thousand_Buddhas">Garden of a Thousand Buddhas</a> in Montana sometime. It is beautiful.
</div>
```

<div class="displayed_code_example">
    <div class="embed-responsive" style="padding-bottom:100px;"><iframe class="embed-responsive-item" src="https://montana-media-arts.github.io/341-work/lectureCode/08/link-hover-01/" frameborder="0" allowfullscreen></iframe></div>
</div>



### `:active`

The `:active` pseudo-class is applied when a user is clicking on an element.

Often this is used to make a button feel more real by slightly changing the color when the user presses it. But this can be used for any pressed effect.

<div id="code-heading">CSS</div>

```css
.parent-element {
    background-color: #fff175;
    min-height: 10em;
}

.button-1 {
    font-size: 1.5em;
    color: #fff;
    background-color: rgb(52, 120, 190);
    border-color: #8f8b8b #383636 #383636 #8f8b8b;
    border-width: 9px 15px 15px 9px;
    border-style: solid;
    position: relative;
    margin: auto;
    top: 1em;
    padding: 1em;
    width: 9em;
    text-align: center;
}

.button-1:hover {
    color: #ffc4ed;
    font-style: italic;
}

.button-1:active {
    color: #fff;
    background-color: rgb(40, 100, 162);
    border-color: #383636 #8f8b8b #8f8b8b #383636;
    border-width: 15px 9px 9px 15px;
}
```


<div id="code-ruler"></div>
<div id="code-heading">HTML</div>

```html
<div class="parent-element">
    <div class="button-1">
        Press me...
    </div>
</div>
```

<div class="displayed_code_example">
<style>
.parent-element {
    background-color: #fff175;
    min-height: 10em;
}

.button-1 {
    font-size: 1.5em;
    color: #fff;
    background-color: rgb(52, 120, 190);
    border-color: #8f8b8b #383636 #383636 #8f8b8b;
    border-width: 9px 15px 15px 9px;
    border-style: solid;
    position: relative;
    margin: auto;
    top: 1em;
    padding: 1em;
    width: 9em;
    text-align: center;
}

.button-1:hover {
    color: #ffc4ed;
    font-style: italic;
}

.button-1:active {
    color: #fff;
    background-color: rgb(40, 100, 162);
    border-color: #383636 #8f8b8b #8f8b8b #383636;
    border-width: 15px 9px 9px 15px;
}

</style>

<div class="parent-element">
<div class="button-1">
    Press me...
</div>
</div>

</div>

| [**[View on GitHub]**](https://github.com/Montana-Media-Arts/341-work/tree/master/lectureCode/08/active-01/index.html) | [**[Live Example]**](https://montana-media-arts.github.io/341-work/lectureCode/08/active-01/) |





# { TODO: }
There are many more pseudo-classes than these discussed so far. To learn more about pseudo-classes, as well as all that exist, please read this following comprehensive article on CSS pseudo-classes;

- [An Ultimate Guide To CSS Pseudo-Classes And Pseudo-Elements](https://www.smashingmagazine.com/2016/05/an-ultimate-guide-to-css-pseudo-classes-and-pseudo-elements/)
