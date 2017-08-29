---
title: CSS Applied
module: 7
---

# CSS Applied

Lets look at some applied CSS, to start understanding how it will effect our webpages.

In lines 13, 21, 27, & 33 elements are selected. Except for the first instance in line 13, the elements are selected using "element selectors". Line 13 uses a class selector (discussed in a few pages).

Within each declaration block, there are multiple style rules, each effecting a specific aspect. Each of the declarations, for each selector, either effects border or background color.

Notice, in the displayed HTML example below the code, how the borders make it easier to visually identify the individual elements.


<div id="code-heading">CSS</div>



{% highlight CSS linenos %}
/* Select the main container 'div' element */
.main-container {
    /* Draw a blue border 2px thick. */
    border-style: solid;
    border-width: 2px;
    border-color: blue;
    /* Color the background grey */
    background: grey;
}
/* Select all h1 elements */
h1 {
    /* Draw an orange border 2px thick around the element. */
    border-style: solid;
    border-color: orange;
    /*Set a unique background color*/
    background: #f0ebeb;
}
/* Select all paragraph elements */
p {
    border-style: solid;
    border-color: yellow;
    background: #ffe4e4;
}
/* Select the strong elements */
strong {
    border-style: solid;
    border-width: 1px;
    border-color: red;
}
/* Select the emphasized elements */
em {
    border-style: solid;
    border-width: 1px;
    border-color: red;
}

{% endhighlight %}

<div id="code-ruler"></div>

<div id="code-heading">HTML</div>

{% highlight html linenos %}
<!-- Div Container -->
<div class="main-container">
    <!-- Heading 1 -->
    <h1 class="main-heading">Heading1</h1>
    <!-- Content Paragraphs -->
    <p class="content-para">A paragraph of <strong>happiness</strong> within a div element.</p>
    <p class="content-para">Another paragraph, that's not <em> as happy,</em> as it follows the other paragraph.</p>
</div>
{% endhighlight %}


<div class="displayed_code_example">
    <style>
        .main-container {
            border-style: solid;
            border-width: 2px;
            border-color: blue;
            background: grey;
        }
        .h1 {
            border-style: solid;
            border-width: 2px;
            border-color: orange;
            background: #fefefe;
        }
        .para {
            border-style: solid;
            border-color: yellow;
            background: #ffeeee;
        }
        strong {
            border-style: solid;
            border-width: 1px;
            border-color: red;
        }
        em {
            border-style: solid;
            border-width: 1px;
            border-color: red;
        }
    </style>

    <div class="main-container">
        <h1 class="h1">Heading1</h1>
        <p class="para">A paragraph of <strong>happiness</strong> within a div element.</p>
        <p class="para">Another paragraph, that's not <em> as happy,</em> as it follows the other paragraph.</p>
    </div>
</div>
