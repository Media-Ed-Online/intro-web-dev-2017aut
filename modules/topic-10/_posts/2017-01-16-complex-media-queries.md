---
title: Complex Media Queries
module: 10
---

# Complex Media Queries

A complex media query is one where the browser looks at _multiple_ conditions to asses when the rules should be applied. This could also be known as a multi-part conditional statement.

For example, we might have a media query that looks to be larger than some size, but also smaller than another size. We could write this like;

<div id="code-heading">CSS</div>

```css
@media (min-width: 500px) and (max-width: 600px) {
    /* Do Something */
}
```

<div class="embed-responsive embed-responsive-16by9"><iframe class="embed-responsive-item" src="https://www.youtube.com/embed/1pUS-g9E-Pg" frameborder="0" allowfullscreen></iframe></div>

You can read more about media queries on the Mozilla Developer Networks site;

- [MDN on Media Queries](https://developer.mozilla.org/en-US/docs/Web/CSS/Media_Queries/Using_media_queries)

#### Media Queries Quiz

<div class="embed-responsive embed-responsive-16by9"><iframe class="embed-responsive-item" src="https://www.youtube.com/embed/0I7Q-5lpCno" frameborder="0" allowfullscreen></iframe></div>

<div class="embed-responsive embed-responsive-16by9"><iframe class="embed-responsive-item" src="https://www.youtube.com/embed/dusZRagGtMU" frameborder="0" allowfullscreen></iframe></div>
