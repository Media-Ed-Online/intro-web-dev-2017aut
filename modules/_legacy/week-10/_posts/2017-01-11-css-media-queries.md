---
title: Media Queries in CSS
module: 10
---

# Media Queries in CSS

In addition to being able to specify various style sheets based on the media width, you can specify within a stylesheet specific parameters based on width conditions. As will be discussed below, this latter technique can increase performance, as your page will rely on fewer stylesheets, thereby reducing the number of resources that must be loaded.

To write a media query within your css stylesheets, you will include the following;

<div id="code-heading">CSS</div>

```css
@media "media conditions"  {
    /* CSS Rules */
    /* Typed Normally */
}
```

You would replace the "media conditions" with your actual media query conditional check. So;

- `screen and (min-width:800px)`
    - This would specify that the inner style rules be applied when the page is "on a screen device" (as opposed to "print"), and the the device width is greater than or equal to 800 pixels.
- `(max-width:450px)`
    - This would specify, that for any media type (screen or print), the following rules would be applied when the device width is less than or equal to 450 pixels.

So, for example, the following would set the text color to green, when the screen size is larger than 600 pixels.

NOTE: How the css rule looks exactly the same is usual within the media query.

<div id="code-heading">CSS</div>

```css
@media (min-width:600px) {
    body {
        color: #00ff00;
    }
}
```


## Media Queries in CSS Discussed

<div class="embed-responsive embed-responsive-16by9"><iframe class="embed-responsive-item" src="https://www.youtube.com/embed/g1Pu_qQs8t0" frameborder="0" allowfullscreen></iframe></div>

<div class="embed-responsive embed-responsive-16by9"><iframe class="embed-responsive-item" src="https://www.youtube.com/embed/gCiCojJGr9w" frameborder="0" allowfullscreen></iframe></div>


#### Quiz

<div class="embed-responsive embed-responsive-16by9"><iframe class="embed-responsive-item" src="https://www.youtube.com/embed/yKfomMEAjRQ" frameborder="0" allowfullscreen></iframe></div>


<br />


- [The quiz link!](http://udacity.github.io/RWDF-samples/quizzes/media-queries-quiz.html)

NOTE: Remember, that you will ignore the "write your code in here request".

##### Answer

<div class="embed-responsive embed-responsive-16by9"><iframe class="embed-responsive-item" src="https://www.youtube.com/embed/vpn3pWEA6Vw" frameborder="0" allowfullscreen></iframe></div>
