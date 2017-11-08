---
title: Intro to Layouts
module: 9
---

# Introduction to Layouts

Using the properties discussed in this week, we can start to build the types of layouts you are likely familiar with seeing on the web.

## Header Example

The following example shows how to use the techniques discussed this week to build a header. This header is made of two basic bars; the top bar is for navigation or a menu, and the second bar presents the sites "identity".

Notice: how the colors for both sections are the inverse of each other in order to provide cohesion amongst the parent elements.

The main container (`header`) has its `padding` and `margin` properties set to `0`, so that there is no space between the header and the container browser page. This is true for the "menu-container" (`.menu-container`) element as well. This makes it possible for it to rest right above the identity bar.

The upper header, or menu bar, is very similar to the example from the position page. It uses `position: inline-block;` to set the menu items (`.menuitem`) next to each other horizontally. It also uses `padding` and `margin` to provide space between each entry.

The hover pseudo-class is used to change the appearance of the elements when a user moves their mouse over them. This allows the user to know that these elements are 'likely' reactive.

There is also a dropdown menu on the last item, that uses the same techniques as discussed earlier.


<br />

The "lower header" (`.lower-header`) serves as a site identity or branding. It contains a stylized version of the site name, as well as a logo image. Both of these have been placed to the hard left and right sides respectively using the `float` property. NOTE: I also set the height of the site logo image within the CSS.

<div id="code-heading">HTML</div>

```html
<header>

    <menu class="menu-container">
        <a href="#" class="menuitem">
                Home</a>
        <a href="#" class="menuitem">
                Contact</a>

        <div class="dropdown">
            <a href="#" class="menuitem">
                Dropdown</a>

            <div class="dropdown-content">
                <a href="#" class="dropdown-item">
                    Dada</a>
                <a href="#" class="dropdown-item">
                    Haha</a>
                <a href="#" class="dropdown-item">
                    Yesterday</a>
                <a href="#" class="dropdown-item">
                    Today</a>
            </div>
        </div>
    </menu>

    <div class="lower-header">
        <div class="site-name">
            Awesome Site
        </div>
        <div class="site-logo">
            <img src="./imgs/buff_icon_right.png" alt="Buff Site Logo Image">
        </div>
    </div>

</header>
```

<div id="code-ruler"></div>
<div id="code-heading">CSS</div>

```css
body {
    font-size: 16pt;
    font-family: 'Helvetica Neue', 'helvetica', sans-serif;
}

header {
    margin: 0;
    padding: 0;
}

.menu-container {
    background-color: #b4b4b4;
    margin: 0;
    padding: 0;
}

.menuitem {
    display: inline-block;
    padding: 0.5em 1em;
    padding-right: 2.5em;
    text-align: left;
    text-decoration: none;
    color: #507aa6;
}

.menuitem:hover, .dropdown:hover {
    color: #fff;
    background-color: #507aa6;
}

.dropdown {
    display: inline-block;
    width: 10%;
    min-width: 100px;
}

.dropdown-content {
    display: none;
    position: absolute;
    border: 1px solid #000;
    margin: 0;
    color: #000;
    background-color: #fff;
    z-index: 1;
}

.dropdown-content a {
    color: #000;
    text-decoration: none;
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
    color: #fff;
    background-color: #507aa6;
}

.lower-header {
    margin: 0;
    background-color: #507aa6;
    height: 80px;
}

.site-name {
    float: left;
    padding: 10px;
    margin-left: 0.25em;
    font-weight: lighter;
    font-size: 2.5em;
    color: #fff;
}

.site-logo {
    font-size: 2.5em;
    float: right;
    padding: 10px;
    margin-right: 0.25em;
}

.site-logo img {
    height: 70px;
}
```

<div class="displayed_code_example">
    <div class="embed-responsive" style="padding-bottom:200px"><iframe class="embed-responsive-item" src="https://montana-media-arts.github.io/341-work/lectureCode/09/float-header-01/" frameborder="0" allowfullscreen></iframe></div>
</div>

| [**[Code Download]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/09/float-header-01/float-header-01.zip) | [**[View on GitHub]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/09/float-header-01/) | [**[Live Example]**](https://montana-media-arts.github.io/341-work/lectureCode/09/float-header-01/) |

#### { TODO: }

Read more about ways to build navigation bars:

- ["CSS Navigation Bars" by w3schools](https://www.w3schools.com/css/css_navbar.asp)

## Body Examples

Study the following layout examples.

#### Body 1 - Center Content Alone

In this first example, the main content or body of a page is presented. This content is presented alone, with ample margins on both sides. It is also centered in the center of the screen.

<div id="code-heading">HTML</div>

```html
<div class="main-container">
    <main>
        <h1>Center Content</h1>
        <p>Occaecat incididunt et nostrud consectetur nostrud quis quis ad velit laboris nulla nostrud eiusmod consequat. Do duis eiusmod et fugiat Lorem velit anim sint do et adipisicing fugiat veniam. Elit Lorem sint commodo quis minim in est. Cupidatat aute consectetur velit Lorem excepteur tempor minim. Ipsum nostrud est veniam labore laboris eiusmod eiusmod laboris minim aliquip anim Lorem. Consectetur fugiat ipsum Lorem commodo occaecat esse occaecat excepteur. Ullamco est laboris enim velit eu laboris pariatur exercitation proident amet.</p>
        <p>Eu eiusmod aliquip amet consequat eu dolore nulla non. Nisi veniam ea dolore sit incididunt commodo nostrud magna veniam consectetur consequat proident sit commodo. Eu proident ullamco excepteur eiusmod eu amet aute sit magna id sit sunt dolor quis. In ut tempor commodo ad consectetur aliqua in in deserunt aliqua do ut. Quis amet qui enim laboris anim dolor proident nulla ipsum proident amet magna ut cillum ea. Ut in magna voluptate proident do consequat magna officia proident occaecat. Enim exercitation velit et ea minim quis adipisicing fugiat duis sit magna.</p>
        <p>Enim elit veniam cupidatat incididunt aliquip incididunt nostrud ea proident ut officia dolor. Elit adipisicing fugiat consectetur velit dolor est fugiat esse ex consectetur nostrud aliqua occaecat deserunt tempor dolore laboris. Cupidatat incididunt culpa qui et veniam deserunt proident ea consectetur.</p>
        <p>Exercitation enim occaecat ex magna duis laborum laborum ex voluptate dolor consequat laborum adipisicing est. Nostrud commodo aute pariatur fugiat aute laborum ut magna esse tempor commodo ullamco dolore occaecat. Eu nisi ipsum amet ipsum nostrud do eiusmod eiusmod consequat sunt. Aliqua do exercitation commodo enim veniam sunt ipsum adipisicing irure proident eiusmod exercitation velit quis duis est ad. Veniam duis est in ut quis nisi enim sit fugiat exercitation aliqua deserunt elit reprehenderit adipisicing.</p>
    </main>
</div>
```


<div id="code-ruler"></div>
<div id="code-heading">CSS</div>

```css
body {
    font-size: 16pt;
    font-family: 'Helvetica Neue', 'helvetica', sans-serif;
    background-color: #aaaaaa;
    padding: 0;
    margin: 0;
}

.main-container {
    margin: auto;
    margin-top: 0;
    padding-top: 0;
    width: 75%;
    min-width: 600px;
    max-width: 960px;
    background-color: #ffffff;
}

.main-container h1 {
    text-align: center;
    font-weight: 200;
    letter-spacing: 0.4em;
    word-spacing: 1em;
    padding: 1em;
    margin-top: 0 !important;
    color: #fff;
    background-color: #507aa6;
    /*border-radius: 20px;*/
}

.main-container p {
    padding: 1em 2em;
    text-indent: 1.5em;
    line-height: 1.5em;
    text-align: justify;
}
```

<div class="displayed_code_example">
    <div class="embed-responsive" style="padding-bottom:600px"><iframe class="embed-responsive-item" src="https://montana-media-arts.github.io/341-work/lectureCode/09/center-body-01/" frameborder="0" allowfullscreen></iframe></div>
</div>

| [**[Code Download]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/09/center-body-01/center-body-01.zip) | [**[View on GitHub]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/09/center-body-01/) | [**[Live Example]**](https://montana-media-arts.github.io/341-work/lectureCode/09/center-body-01/) |


#### Body Example 2 (with an aside)

In this next example, there is an "aside" containing secondary information. This is placed using the float property, so that the main content can "flow" around it, after the aside "is finished".

<div id="code-heading">HTML</div>

```html
<div class="main-container">

    <aside class="content-side">
        <div class="aside-head">
            Look at This Info!
        </div>
        <div class="aside-text">
            <p>Something incredibly profound that adds to the users experience.</p>
            <p>This is some amazing stuff over here. I reeally think it adds meaning to the site.</p>
        </div>
        <div class="aside-img">
            <img src="./imgs/buff_icon_right.png" alt="Buff Site Logo">
        </div>
    </aside>


    <main>
        <h1>Center Content</h1>
        <p>Occaecat incididunt et nostrud consectetur nostrud quis quis ad velit laboris nulla nostrud eiusmod consequat. Do duis eiusmod et fugiat Lorem velit anim sint do et adipisicing fugiat veniam. Elit Lorem sint commodo quis minim in est. Cupidatatm aute consectetur velit Lorem excepteur tempor minim. Ipsum nostrud est veniam labore laboris eiusmod eiusmod laboris minim aliquip anim Lorem. Consectetur fugiat ipsum Lorem commodo occaecat esse occaecat excepteur. Ullamco est laboris enim velit eu laboris pariatur exercitation proident amet.</p>
        <p>Eu eiusmod aliquip amet consequat eu dolore nulla non. Nisi veniam ea dolore sit incididunt commodo nostrud magna veniam consectetur consequat proident sit commodo. Eu proident ullamco excepteur eiusmod eu amet aute sit magna id sit sunt dolor quis. In ut tempor commodo ad consectetur aliqua in in deserunt aliqua do ut. Quis amet qui enim laboris anim dolor proident nulla ipsum proident amet magna ut cillum ea. Ut in magna voluptate proident do consequat magna officia proident occaecat. Enim exercitation velit et ea minim quis adipisicing fugiat duis sit magna.</p>
        <p>Enim elit veniam cupidatat incididunt aliquip incididunt nostrud ea proident ut officia dolor. Elit adipisicing fugiat consectetur velit dolor est fugiat esse ex consectetur nostrud aliqua occaecat deserunt tempor dolore laboris. Cupidatat incididunt culpa qui et veniam deserunt proident ea consectetur.</p>
        <p>Exercitation enim occaecat ex magna duis laborum laborum ex voluptate dolor consequat laborum adipisicing est. Nostrud commodo aute pariatur fugiat aute laborum ut magna esse tempor commodo ullamco dolore occaecat. Eu nisi ipsum amet ipsum nostrud do eiusmod eiusmod consequat sunt. Aliqua do exercitation commodo enim veniam sunt ipsum adipisicing irure proident eiusmod exercitation velit quis duis est ad. Veniam duis est in ut quis nisi enim sit fugiat exercitation aliqua deserunt elit reprehenderit adipisicing.</p>
    </main>

</div>
```


<div id="code-ruler"></div>
<div id="code-heading">CSS</div>

```css
body {
    font-size: 16pt;
    font-family: 'Helvetica Neue', 'helvetica', sans-serif;
    /*background-color: #aaaaaa;*/
    background-color: #fff;
    padding: 0;
    margin: 0;
}

.main-container {
    margin: auto;
    margin-top: 0;
    padding-top: 0;
    min-width: 600px;
    max-width: 1280px;
    background-color: #ffffff;
    clear: both;
}

.main-container main {
    margin: 0;
    padding: 0;
    /*float: left;*/
    height: 100%;
    background-color: #ffffff;
}

.main-container h1 {
    text-align: center;
    font-weight: lighter;
    letter-spacing: 0.4em;
    word-spacing: 1em;
    padding: 2em 0 1em 0;
    margin-top: 0 !important;
    color: #000;
    background-color: #fff;
    /*border-radius: 20px;*/
}

.main-container p {
    padding: 1em 2em;
    text-indent: 1.5em;
    line-height: 1.5em;
    text-align: justify;
}

.main-container aside.content-side {
    float: right;
    margin: 2em;
    margin-top: 4em;
    padding: 0;
    width: 25%;
    color: #fff;
    background-color: #507aa6;
    font-weight: lighter;
}

aside .aside-head {
    font-size: 1.5em;
    text-align: center;
    padding: 1em;
    background-color: #bf628c;
}

aside .aside-text {
    padding-top: 2em;
    padding-bottom: 2em;
}

aside .aside-text p {
    font-style: italic;
    padding: 0.25em 1em;
    margin: 0;
    text-align: left;
}

aside .aside-img img {
    display: block;
    padding: 1em;
    margin: auto;
}
```

<div class="displayed_code_example">
    <div class="embed-responsive" style="padding-bottom:600px"><iframe class="embed-responsive-item" src="https://montana-media-arts.github.io/341-work/lectureCode/09/float-body-with-aside-01/" frameborder="0" allowfullscreen></iframe></div>
</div>

| [**[Code Download]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/09/float-body-with-aside-01/float-body-with-aside-01.zip) | [**[View on GitHub]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/09/float-body-with-aside-01/) | [**[Live Example]**](https://montana-media-arts.github.io/341-work/lectureCode/09/float-body-with-aside-01/) |


#### Body Example 3 (with a side menu)

In this next example, the left 25% of the screen is used for a vertical menu, while the right 75% is the main content.

As with the above examples, this is accomplished using the float property, along with specifically stating the width of each section as a percentage.


<div id="code-heading">HTML</div>

```html
<div class="main-container">
    <menu>
        <div class="site-name">
            Awesome Site
        </div>
        <div class="side-menu-item">
            <a href="#" class="side menuitem">
                    Home</a>

            <div class="side dropdown">
                <a href="#" class="side menuitem">
                    + Dropdown</a>

                <div class="dropdown-content">
                    <a href="#" class="side menuitem dropdown-item">
                        Dada</a>
                    <a href="#" class="side menuitem dropdown-item">
                        Haha</a>
                    <a href="#" class="side menuitem dropdown-item">
                        Yesterday</a>
                    <a href="#" class="side menuitem dropdown-item">
                        Today</a>
                </div>
            </div>

            <a href="#" class="side menuitem">
                Contact</a>
        </div>
    </menu>

    <main>
        <h1>Center Content</h1>
        <p>Occaecat incididunt et nostrud consectetur nostrud quis quis ad velit laboris nulla nostrud eiusmod consequat. Do duis eiusmod et fugiat Lorem velit anim sint do et adipisicing fugiat veniam. Elit Lorem sint commodo quis minim in est. Cupidatat aute consectetur velit Lorem excepteur tempor minim. Ipsum nostrud est veniam labore laboris eiusmod eiusmod laboris minim aliquip anim Lorem. Consectetur fugiat ipsum Lorem commodo occaecat esse occaecat excepteur. Ullamco est laboris enim velit eu laboris pariatur exercitation proident amet.</p>
        <p>Eu eiusmod aliquip amet consequat eu dolore nulla non. Nisi veniam ea dolore sit incididunt commodo nostrud magna veniam consectetur consequat proident sit commodo. Eu proident ullamco excepteur eiusmod eu amet aute sit magna id sit sunt dolor quis. In ut tempor commodo ad consectetur aliqua in in deserunt aliqua do ut. Quis amet qui enim laboris anim dolor proident nulla ipsum proident amet magna ut cillum ea. Ut in magna voluptate proident do consequat magna officia proident occaecat. Enim exercitation velit et ea minim quis adipisicing fugiat duis sit magna.</p>
        <p>Enim elit veniam cupidatat incididunt aliquip incididunt nostrud ea proident ut officia dolor. Elit adipisicing fugiat consectetur velit dolor est fugiat esse ex consectetur nostrud aliqua occaecat deserunt tempor dolore laboris. Cupidatat incididunt culpa qui et veniam deserunt proident ea consectetur.</p>
        <p>Exercitation enim occaecat ex magna duis laborum laborum ex voluptate dolor consequat laborum adipisicing est. Nostrud commodo aute pariatur fugiat aute laborum ut magna esse tempor commodo ullamco dolore occaecat. Eu nisi ipsum amet ipsum nostrud do eiusmod eiusmod consequat sunt. Aliqua do exercitation commodo enim veniam sunt ipsum adipisicing irure proident eiusmod exercitation velit quis duis est ad. Veniam duis est in ut quis nisi enim sit fugiat exercitation aliqua deserunt elit reprehenderit adipisicing.</p>
    </main>
</div>
```


<div id="code-ruler"></div>
<div id="code-heading">CSS</div>

```css
body {
    font-size: 16pt;
    font-family: 'Helvetica Neue', 'helvetica', sans-serif;
    /*background-color: #aaaaaa;*/
    background-color: #fff;
    padding: 0;
    margin: 0;
}

.main-container {
    margin: auto;
    margin-top: 0;
    padding-top: 0;
    min-width: 600px;
    max-width: 1280px;
    background-color: #ffffff;
    clear: both;
}

.main-container menu {
    margin: 0;
    padding: 0;
    float: left;
    width: 25%;
    height: 1000px;
    background-color: #808080;
}

.site-name {
    padding: 1em 0.5em;
    margin-left: 0;
    font-weight: lighter;
    font-size: 1.5em;
    color: #fff;
    background-color: #507aa6;
}

.site-logo {
    font-size: 2.5em;
    float: right;
    padding: 10px;
    margin-right: 0.25em;
}

.site-logo img {
    height: 70px;
}

.side.menuitem {
    display: block;
    font-size: 1em;
    font-weight: lighter;
    padding: 0.5em;
    margin: 0.1em 0;
    text-decoration: none;
    background-color: #73d2a2;
    color: #fff;
}

.side.menuitem:hover {
    background-color: #bf628c;
    color: #fff;
}

.dropdown-content {
    display: none;
}

.dropdown:hover .dropdown-content {
    display: block;
}

.side.menuitem.dropdown-item {
    font-size: 0.8em;
    padding-left: 2em;
    margin-top: 0.05em;
    background-color: #bf628c;
    color: #fff;
}

.dropdown:hover .dropdown-content .side.menuitem.dropdown-item:hover {
    background-color: #fff;
    color: #bf628c;
}

.main-container main {
    margin: 0;
    padding: 0;
    float: left;
    width: 75%;
    min-width: 399px;
    height: 100%;
    background-color: #ffffff;
}

.main-container h1 {
    text-align: center;
    font-weight: lighter;
    letter-spacing: 0.4em;
    word-spacing: 1em;
    padding: 2em 0 1em 0;
    margin-top: 0 !important;
    color: #000;
    background-color: #fff;
    /*border-radius: 20px;*/
}

.main-container p {
    padding: 1em 2em;
    text-indent: 1.5em;
    line-height: 1.5em;
    text-align: justify;
}
```

<div class="displayed_code_example">
    <div class="embed-responsive" style="padding-bottom:600px"><iframe class="embed-responsive-item" src="https://montana-media-arts.github.io/341-work/lectureCode/09/float-body-with-side-menu-01/" frameborder="0" allowfullscreen></iframe></div>
</div>

| [**[Code Download]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/09/float-body-with-side-menu-01/float-body-with-side-menu-01.zip) | [**[View on GitHub]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/09/float-body-with-side-menu-01/) | [**[Live Example]**](https://montana-media-arts.github.io/341-work/lectureCode/09/float-body-with-side-menu-01/) |

## All Together

Finally, lets take elements from all of the above and make a simple webpage.

This page has a header, side menu, main content section, an aside, and footer.

Rather than try to print out all of the code for this example, you should view it on github, or download it, via the links below the example. 

<div class="displayed_code_example">
    <div class="embed-responsive" style="padding-bottom:800px"><iframe class="embed-responsive-item" src="https://montana-media-arts.github.io/341-work/lectureCode/09/layout-example-01/" frameborder="0" allowfullscreen></iframe></div>
</div>

| [**[Code Download]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/09/layout-example-01/layout-example-01.zip) | [**[View on GitHub]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/09/layout-example-01/) | [**[Live Example]**](https://montana-media-arts.github.io/341-work/lectureCode/09/layout-example-01/) |
