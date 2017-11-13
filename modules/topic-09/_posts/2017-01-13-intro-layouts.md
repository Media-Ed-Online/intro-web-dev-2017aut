---
title: Intro to Layouts
module: 09
---

## Introduction to Layouts:
<img src="./../../../img/arrow-divider.svg" style="width: 75px; border: none;" />

Using the properties discussed in this week, we can start to build the types of layouts you are likely familiar with seeing on the web.

### Header Example

The following example shows how to use the techniques discussed this week to build a header. This header is made of two basic bars; the top bar is for navigation or a menu, and the second bar presents the site's "identity".

**NOTE:** How the colors for both sections are the inverse of each other in order to provide cohesion amongst the parent elements.

The main container (`header`) has its `padding` and `margin` properties set to `0`, so that there is no space between the header and the container browser page. This is true for the "menu-container" (`.menu-container`) element as well. This makes it possible for it to rest right above the identity bar.

The upper header, or menu bar, is very similar to the example from the position page. It uses `position: inline-block;` to set the menu items (`.menuitem`) next to each other horizontally. It also uses `padding` and `margin` to provide space between each entry.

The hover pseudo-class is used to change the appearance of the elements when a user moves their mouse over them. This allows the user to know that these elements are 'likely' reactive.

There is also a dropdown menu on the last item, that uses the same techniques as discussed earlier.


<br />

The "lower header" (`.lower-header`) serves as a site identity or branding. It contains a stylized version of the site name, as well as a logo image. Both of these have been placed to the hard left and right sides respectively using the `float` property.

**NOTE:** I also set the height of the site logo image within the CSS.

<div class="pen-group">
  <p data-height="600" data-theme-id="30567" data-slug-hash="xPgvgy" data-default-tab="html,css" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Topic-09] Layout, Pt. 1" class="codepen"></p>
  <script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>
  <iframe src="{{site.baseurl}}/modules/topic-09/layout-ex1.html" width="100%" height="600" frameborder="" allowfullscreen style="border: 1px solid #B3B3B3;"></iframe>
</div>


### Body Examples

Study the following layout examples:

#### _Body Example 1 - Center Content Alone_

In this first example, the main content or body of a page is presented. This content is presented alone, with ample margins on both sides. It is also centered in the center of the screen.

<div class="pen-group">
  <p data-height="400" data-theme-id="30567" data-slug-hash="dZvbmO" data-default-tab="html,css" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Topic-09] Layout, Pt. 2" class="codepen"></p>

  <div class="pen-result displayed_code_example_pen" style="height: 600px; overflow: auto;">
    <style>
        .body-1 {
            font-size: 16pt;
            font-family: 'Helvetica Neue', 'helvetica', sans-serif;
            background-color: #27435C;
            padding: 0;
            margin: 0;
            color: #27435C;
        }
        .main-container-1 {
            margin: auto;
            margin-top: 0;
            padding-top: 0;
            width: 75%;
            background-color: #ffffff;
        }
        .main-container-1 h1 {
            text-align: center;
            font-weight: 200;
            letter-spacing: 0.4em;
            word-spacing: 1em;
            padding: 1em 0em;
            margin-top: 0 !important;
            color: #fff;
            background-color: #F15F50;
        }
        .main-container-1 p {
            padding: 1em 2em;
            text-indent: 1.5em;
            line-height: 1.5em;
            text-align: justify;
        }
    </style>
    <div class="body-1">
      <div class="main-container-1">
          <main>
              <h1>Center Content</h1>
              <p>Occaecat incididunt et nostrud consectetur nostrud quis quis ad velit laboris nulla nostrud eiusmod consequat. Do duis eiusmod et fugiat Lorem velit anim sint do et adipisicing fugiat veniam. Elit Lorem sint commodo quis minim in est. Cupidatat aute consectetur velit Lorem excepteur tempor minim. Ipsum nostrud est veniam labore laboris eiusmod eiusmod laboris minim aliquip anim Lorem. Consectetur fugiat ipsum Lorem commodo occaecat esse occaecat excepteur. Ullamco est laboris enim velit eu laboris pariatur exercitation proident amet.</p>
              <p>Eu eiusmod aliquip amet consequat eu dolore nulla non. Nisi veniam ea dolore sit incididunt commodo nostrud magna veniam consectetur consequat proident sit commodo. Eu proident ullamco excepteur eiusmod eu amet aute sit magna id sit sunt dolor quis. In ut tempor commodo ad consectetur aliqua in in deserunt aliqua do ut. Quis amet qui enim laboris anim dolor proident nulla ipsum proident amet magna ut cillum ea. Ut in magna voluptate proident do consequat magna officia proident occaecat. Enim exercitation velit et ea minim quis adipisicing fugiat duis sit magna.</p>
              <p>Enim elit veniam cupidatat incididunt aliquip incididunt nostrud ea proident ut officia dolor. Elit adipisicing fugiat consectetur velit dolor est fugiat esse ex consectetur nostrud aliqua occaecat deserunt tempor dolore laboris. Cupidatat incididunt culpa qui et veniam deserunt proident ea consectetur.</p>
              <p>Exercitation enim occaecat ex magna duis laborum laborum ex voluptate dolor consequat laborum adipisicing est. Nostrud commodo aute pariatur fugiat aute laborum ut magna esse tempor commodo ullamco dolore occaecat. Eu nisi ipsum amet ipsum nostrud do eiusmod eiusmod consequat sunt. Aliqua do exercitation commodo enim veniam sunt ipsum adipisicing irure proident eiusmod exercitation velit quis duis est ad. Veniam duis est in ut quis nisi enim sit fugiat exercitation aliqua deserunt elit reprehenderit adipisicing.</p>
          </main>
      </div>
    </div>
  </div>
</div>



#### _Body Example 2 - Add an Aside_

In this next example, there is an "aside" containing secondary information. This is placed using the float property, so that the main content can "flow" around it, after the aside "is finished".

<div class="pen-group">
  <p data-height="400" data-theme-id="30567" data-slug-hash="POpRYe" data-default-tab="html,css" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Topic-09] Layout, Pt. 2" class="codepen"></p>

  <div class="pen-result displayed_code_example_pen" style="height: 600px; overflow: auto;">
    <style>
        body-2 {
            font-size: 16pt;
            font-family: 'Helvetica Neue', 'helvetica', sans-serif;
            background-color: #fff;
            padding: 0;
            margin: 0;
        }

        .main-container-2 {
            margin: auto;
            margin-top: 0;
            padding-top: 0;
            min-width: 600px;
            max-width: 1280px;
            background-color: #fff;
            clear: both;
        }

        .main-container-2 main {
            margin: 0;
            padding: 0;
            /*float: left;*/
            height: 100%;
            background-color: #ffffff;
        }

        .main-container-2 h1 {
            text-align: center;
            font-weight: lighter;
            letter-spacing: 0.4em;
            word-spacing: 1em;
            padding: 2em 0 1em 0;
            margin-top: 0 !important;
            color: #000;
            background-color: #fff;
            font-size: 200%;
        }

        .main-container-2 p {
            padding: 1em 2em;
            text-indent: 1.5em;
            line-height: 1.5em;
            text-align: justify;
            color: #27435C;
        }

        .main-container-2 aside.content-side-2 {
            float: right;
            margin: 2em;
            margin-top: 4em;
            padding: 0;
            width: 30%;
            color: #fff;
            background-color: #F15F50;
            font-weight: lighter;
        }

        aside .aside-head-2 {
            font-size: 1.5em;
            text-align: center;
            padding: 1em;
            background-color: #27435C;
            margin-top: 0;
        }

        aside .aside-text-2 {
            padding-top: 2em;
            padding-bottom: 2em;
        }

        aside .aside-text-2 p {
            font-style: italic;
            padding: 0.25em 1em;
            margin: 0;
            text-align: left;
            color: #fff;
        }

        aside .aside-img-2 {
           border: 3px dashed #27435C;
           border-radius: 500px;
           background-color: #fff;
           width: 75%;
           margin: auto;
           margin-bottom: 2em;
        }

        aside .aside-img-2 img {
            display: block;
            padding: 1%;
            position: relative;
            margin: 1.5em auto;
            width: 50%;
            border: none;
        }
    </style>
    <body class="body-2">
       <div class="main-container-2">
          <aside class="content-side-2">
             <div class="aside-head-2">
                Look at This Info!
             </div>
             <div class="aside-text-2">
                <p>Something incredibly profound that adds to the users experience.</p>
                <p>This is some amazing stuff over here. I really think it adds meaning to the site.</p>
             </div>
             <div class="aside-img-2">
                <img src="https://tinyurl.com/tag-logo-png" alt="Shopping Site Logo Image">
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
    </body>
  </div>
</div>


#### _Body Example 3 - Add a Side Menu_

In this next example, the left 25% of the screen is used for a vertical menu, while the right 75% is the main content.

As with the above examples, this is accomplished using the float property, along with specifically stating the width of each section as a percentage.

<div class="pen-group">
  <p data-height="400" data-theme-id="30567" data-slug-hash="POpRxL" data-default-tab="html,css" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Topic-09] Layout, Pt. 3" class="codepen"></p>
  <iframe src="{{site.baseurl}}/modules/topic-09/layout-ex2.html" width="100%" height="600" frameborder="" allowfullscreen style="border: 1px solid #B3B3B3;"></iframe>
</div>

### All Together

Finally, let's take elements from all of the above and make a simple webpage!

This page has a header, side menu, main content section, an aside, and footer.

Rather than try to print out all of the code for this example, you should [view it in your browser]({{site.baseurl}}/modules/topic-09/layout-ex3/), or [download the files for yourself]({{site.baseurl}}/modules/topic-09/files/layout-ex3.zip).

<div class="pen-group">
  <p data-height="600" data-theme-id="30567" data-slug-hash="OOpwga" data-default-tab="html,css" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Topic-09]  Full Site Layout" class="codepen"></p>
  <iframe src="{{site.baseurl}}/modules/topic-09/layout-ex3/" width="100%" height="600" frameborder="" allowfullscreen style="border: 1px solid #B3B3B3;"></iframe>
</div>


# { TODO: }
1. <a href="{{site.baseurl}}/modules/topic-09/layout-ex3/" target="_blank">Open the example in a separate tab</a> to see it in full. Be sure to view the source code!
2. Read more about ways to build "[CSS Navigation Bars](https://www.w3schools.com/css/css_navbar.asp)" from W3Schools.
3. Read pages 377-405 of Chapter 15 in [Duckett](https://github.com/Media-Ed-Online/intro-web-dev/issues/3).
