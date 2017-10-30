---
title: Pseudo-Elements
module: 08
---

## First Letter & First Line
<img src="./../../../img/arrow-divider.svg" style="width: 75px; border: none;" />

CSS includes a number of _pseudo_ things. The first type of pseudo thing we will discuss are "**pseudo-elements**".

Pseudo-elements allow for the selection of content, as if it were a separate element, without having to mark it up as such in the HTML.

Two pseudo elements that are made available with CSS are "first letter" and "first line". Respectively, these allow for the selection of the first letter or first line, in an element's text. This selection can then be used to alter the appearance or display of just the first letter or line.

The selectors for first letter and line are:

<div id="code-heading">CSS</div>
```css
selector::first-letter {}
selector::first-line {}

/*The word selector in the above is replaced with
the normal CSS selectors used to identify elements.*/

p::first-letter {color: green; font-size: 1.25em}
```


##### Example 1

In the following, the first letter and line of a div element are selected and altered.

<div class="pen-group">
  <p data-height="400" data-theme-id="30567" data-slug-hash="BmyNqx" data-default-tab="html,css" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Topic-08] Text Pseudos, Pt. 1" class="codepen"></p>
  <script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>

  <div class="pen-result displayed_code_example_pen">
    <style>
      .text-element {
         font-size: 1.5em;
         text-indent: 30px;
      }
      .text-element::first-letter {
         color: yellow;
         font-weight: bolder;
      }
      .text-element::first-line {
          background-color: #1CCDCA;
      }
    </style>
    <div class="text-element">
    Do voluptate velit officia et voluptate cupidatat eiusmod nostrud consequat. Est dolore laborum eiusmod culpa ut exercitation nostrud Lorem in sint et tempor ea incididunt. In non irure pariatur in mollit id fugiat tempor dolore ut nisi minim irure aliqua anim. Irure dolore et cillum non culpa quis amet. </div>
  </div>
</div>


##### Example 2

In the following example, the same technique of using the first letter selector is applied to create a large letter, like might occur in a children's book.

<div class="pen-group">
  <p data-height="600" data-theme-id="30567" data-slug-hash="JOodqR" data-default-tab="html,css" data-user="Media-Ed-Online" data-embed-version="2" data-pen-title="[Topic-08] Text Pseudos, Pt. 2" class="codepen"></p>
  <script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>

  <div class="pen-result displayed_code_example_pen">
    <style>
      @import url('https://fonts.googleapis.com/css?family=Gentium+Book+Basic:400,700');
      .rumple-body {
          background-color: rgb(147, 12, 76);
      }
      .parent-container {
          padding: 1em 2em;
      }
      .text-block {
          font-family: 'Gentium Book Basic', serif;
          font-weight: 400;
          font-size: 1.5em;
          padding: 1em;
          margin: 1em;
          background-color: #fff;
          text-indent: 1.5em;
          line-height: 1.5em;
      }
      .text-block p:first-child {
          text-indent: 0;
      }
      /*.text-block::first-letter doesn't work*/
      .first-letter {
          font-size: 4em;
          font-weight: 700;
          color: rgb(11, 44, 126);
      }
      .spoken {
         font-style: italic;
      }
      #first-offer {
         color: rgb(147, 12, 76);
         text-decoration: underline
      }
    </style>
    <div class="rumple-body">
      <div class="parent-container">
        <div class="text-block">
          <p><span class="first-letter">T</span>hereupon he himself locked up the room, and left her in it alone. So there sat the poor miller's daughter, and for the life of her could not tell what to do, she had no idea how straw could be spun into gold, and she grew more and more frightened, until at last she began to weep.</p>
          <p>But all at once the door opened, and in came a little man, and said, <span class="spoken">"Good evening, mistress miller, why are you crying so?"</span></p>
          <p><span class="spoken">"Alas,"</span> answered the girl, <span class="spoken">"I have to spin straw into gold, and I do not know how to do it."</span></p>
          <p><span class="spoken" id="first-offer">"What will you give me,"</span> said the manikin, <span class="spoken">"if I do it for you?"</span></p>
        </div>
      </div>
    </div>
  </div>
</div>


# { TODO: }
Read page 289 of Chapter 12 in [Duckett](https://github.com/Media-Ed-Online/intro-web-dev/issues/3).
