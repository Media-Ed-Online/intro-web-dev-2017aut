---
title: Display Hidden
module: 9
---

# Hide with Display

The display property can also be used to 'hide' elements. At first, it may seem difficult to understand why it would be useful to hide an element, but this is done often in order to create "drop-down menus" or "hidden tips" type content.

To hide an element, set the `display` properties value to `none`. To get it to appear, you create a selector made up of the parent container and element in question, with the `:hover` pseudo-class added to the parent.

```css
.child-class-to-unhide {
    display: none;
}
.parent-container:hover .child-class-to-unhide {
    display: block;
}
```

In the following example, this exact technique is used to create an "additional information" type box.

<div id="code-heading">HTML</div>

```html
<div class="container">
    <div class="tip-header">
        Hover over me for more information...

    </div>
    <div class="hidden-content">
        This is some hidden information,
        that serves to further enlighten your end-user.
    </div>
</div>
```


<div id="code-ruler"></div>
<div id="code-heading">CSS</div>

```css
.container {
    font-family: sans-serif;
    font-size: 16pt;
    width: 100%;
    min-width: 200px;
    max-width: 500px;
    background-color: #3eb4da;
}

.tip-header {
    font-size: 1.5em;
    padding: 1em;
    text-align: center;
    color: #fff;
    background-color: #18516e;
}


.hidden-content {
    display: none;
    font-size: 1em;
    padding: 1em;
}

.container:hover .hidden-content {
    display: block;
}
```

<div class="displayed_code_example">
<style>
.example-container {
    font-family: sans-serif;
    font-size: 16pt;
    width: 100%;
    min-width: 200px;
    max-width: 500px;
    background-color: #3eb4da;
}

.tip-header {
    font-size: 1.5em;
    padding: 1em;
    text-align: center;
    color: #fff;
    background-color: #18516e;
}


.example-container .hidden-content {
    display: none;
    font-size: 1em;
    padding: 1em;
}

.example-container:hover .hidden-content {
    display: block;
}
</style>

<div class="example-container">
    <div class="tip-header">
        Hover over me for more information...

    </div>
    <div class="hidden-content">
        This is some hidden information,
        that serves to further enlighten your end-user.
    </div>
</div>

</div>

| [**[Code Download]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/09/display-block-01/display-block-01.zip) | [**[View on GitHub]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/09/display-block-01/) | [**[Live Example]**](https://montana-media-arts.github.io/341-work/lectureCode/09/display-block-01/) |




## Used for Dropdown Menus

This same technique can be used for to create dropdown menus.

The following code is one solution to creating a horizontal menu with a dropdown. Notice in line 33, that the content is hidden. Lines 47-49, cause the menu to be displayed, and lines 32-62 are used to present and style the dropdown menu.

Please study the following code to understand it better. You should also download the code and play with it via the links under the example.

<div id="code-heading">HTML</div>

{% highlight html linenos %}
<header class="">
    <div class="menu-item">
        <a href="#">Home</a></div>
    <div class="menu-item">
        <a href="#">About</a></div>
    <div class="menu-item dropdown">
        <a href="#">Dropdown</a>
        <div class="dropdown-content">
            <div class="dropdown-item">
                <a href="#">Dada</a></div>
            <div class="dropdown-item">
                <a href="#">Haha</a></div>
            <div class="dropdown-item">
                <a href="#">Yesterday</a></div>
            <div class="dropdown-item">
                <a href="#">Today</a></div>
        </div>
    </div>
</header>
{% endhighlight %}


<div id="code-ruler"></div>
<div id="code-heading">CSS</div>


{% highlight css linenos %}
header {
    background-color: #26272b;
    font-family: sans-serif;
    font-size: 16pt;
    text-transform: uppercase;
    margin: 0;
    height: 2.15em;
}

.menu-item {
    display: inline-block;
    margin: 0 0;
    min-width: 8em;
    text-align: center;
    background-color: #26272b;
    padding: 0.5em 0;
}

.menu-item a {
    color: #fff;
    text-decoration: none;
}

.menu-item:hover {
    background-color: #673667;
}

.dropdown {
    display: inline-block;
}

.dropdown-content {
    display: none;
    position: absolute;
    border: 1px solid #000;
    margin: 0;
    margin-top: 0.5em;
    color: #000;
    background-color: #fff;
    z-index: 1;
}

.dropdown-content a {
    color: #000;
}

.dropdown:hover .dropdown-content {
    display: block;
}

.dropdown-item {
    display: block;
    text-align: left;
    margin: 0;
    padding: 0.5em;
    min-width: 7em;
}

.dropdown-item:hover, .dropdown-item:hover a {
    color: #673667;
    background-color: #a2a2a2;
}
{% endhighlight %}

<div class="displayed_code_example">
    <div class="embed-responsive" style="padding-bottom:250px"><iframe class="embed-responsive-item" src="https://montana-media-arts.github.io/341-work/lectureCode/09/drop-down-menu-01/" frameborder="0" allowfullscreen></iframe></div>
</div>


| [**[Code Download]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/09/drop-down-menu-01/drop-down-menu-01.zip) | [**[View on GitHub]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/09/drop-down-menu-01/) | [**[Live Example]**](https://montana-media-arts.github.io/341-work/lectureCode/09/drop-down-menu-01/) |


## { TODO: }

Please study the following page on menus from w3schools.

- [CSS Navigation Bar](https://www.w3schools.com/css/css_navbar.asp)



## { TODO: }

You should also read Chapter 13 on Boxes from the Duckett.
