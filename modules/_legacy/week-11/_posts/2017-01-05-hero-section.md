---
title: Hero Image
module: 11
---

# The Hero Image

One of the current trends in web development, that has been ongoing for a number of years now, is the "Hero Image". A hero image is effective for the reason that, "a picture is worth a thousand words".

A hero image takes a large image, of high quality, that is as wide as the browser, and often as tall, and places minimal text over it (usually just a header and maybe navigation). This serves to add "depth" to a site, and visually direct the view as to what the site might be about.

To get a better idea about the diversity and possibility of the hero image, check out the following articles, which present and discuss sites utilizing hero images;

- ["The Power Of Hero Image Design: 35 Striking Case Studies" by Mary Stribley](https://designschool.canva.com/blog/hero-images/)
- ["Exploring the Hero Image Trend in Web Design" by Jake Rocheleau](https://envato.com/blog/exploring-hero-image-trend-web-design/)
- ["Using background and hero images on websites" by Brenda Stokes Barron](https://envato.com/blog/use-background-hero-images-websites/)

## Details

The hero image utilizes the `background-image:` property. Set an elements background using this property. Then set this element to take up the full width of a screen. Then depending on your image, specify if the hero image should always be a certain size, or whether its height should instead stay in relation to the width of the screen.

Finally, lay your other text-based (heading, sub-heading, short description, and/or navigation) over the image. This can be done using `position: absolute;` or by including these elements as children to the containing hero image element.

Notice in the following example, that the basic operation of including the hero image occurs in the `.hero` class.

Also notice how this example was made responsive with the use of media queries that adjust text size and element sizing based on browser width.

<div id="code-heading">HTML</div>

```html
<div class="hero">
            <div class="title">
        <h1>Chateua Musića</h1>
        <h2>Fine Al Fresco Dining</h2>
        <h2>On the private porch</h2>
        <div class="nav">
            <a href="#"><div class="nav-item">Hours</div></a>
            <a href="#"><div class="nav-item">About</div></a>
            <a href="#"><div class="nav-item">Location</div></a>
            <a href="#"><div class="nav-item">Menus</div></a>
        </div>
    </div>
</div>
```


<div id="code-ruler"></div>
<div id="code-heading">CSS</div>

```css
body {
    padding: 0;
    margin: 0;

}

.hero {
    /* the 'vh' unit asks the browser to */
    /* return the height of the viewport */
    /* we can then use that to set the height of an element */
    height: 100vh;
    background-image: url("imgs/hero-image-2.jpg");
    /*background-image: url("imgs/hero-image.jpg");*/
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
}

.hero .title {
    font-size: 22pt;
    color: #fff;
    float: right;
    margin-top: 170px;
    margin-left: 1em;
    margin-right: 1em;
    padding: 2em;
    text-align: center;
    background-color: rgba(120, 120, 120, 0.3);
}

.title h1 {
    font-family: 'Princess Sofia', cursive;
    font-size: 2.5em;
    letter-spacing: 0.2em;
}

.title h2 {
    font-family: 'Josefin Sans', sans-serif;
    font-weight: 300;
    font-style: italic;
    line-height: 0.5em;
}

.hero .nav {
    font-family: 'Josefin Sans', sans-serif;
    font-style: italic;
    font-weight: 300;
    color: #fff;
    margin-top: 2em;
    font-size: 1.5em;
    display: flex;
    flex-direction: row;
}

.hero .nav a {
    flex-grow: 1;
    color: #fff;
    text-decoration: none;
}

.hero .nav-item {
    font-size: 0.5em;
    padding: 0.5em 1em;
    margin: 0 0.5em;
    text-align: center;
    border: 1px solid #d9d9d9;
    border-width: 1px 0;
}

.hero .nav-item:hover {
    color: #fff;
    background-color: rgba(207, 200, 222, 0.5);
}


@media (max-width: 865px) {
    .hero .title {
        font-size: 18pt;
    }
}

@media (max-width: 585px) {
    .hero .title {
        font-size: 14pt;
        margin: 0;
        margin-top: 50px;
    }
}

@media (max-width: 445px) {
    .hero .title {
        font-size: 12pt;
    }
}
```

<div class="displayed_code_example">
    <div class="embed-responsive" style="padding-bottom:800px"><iframe class="embed-responsive-item" src="https://montana-media-arts.github.io/341-work/lectureCode/11/hero-image-01/" frameborder="0" allowfullscreen></iframe></div>
</div>

| [**[Code Download]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/11/hero-image-01/hero-image-01.zip) | [**[View on GitHub]**](https://github.com/Montana-Media-Arts/341-work/raw/master/lectureCode/11/hero-image-01/) | [**[Live Example]**](https://montana-media-arts.github.io/341-work/lectureCode/11/hero-image-01/) |


## More Details

For more resources on implementing this technique please read;

- ["How TO - Hero Image" by w3schools](https://www.w3schools.com/howto/howto_css_hero_image.asp)
- ["Perfect Full Page Background Image" by Chris Coyier](https://css-tricks.com/perfect-full-page-background-image/)
- [Basic "Full Height hero image" Code Pen](https://codepen.io/pooley182/pen/vEYPaR)
-

Also, when creating hero images, you will need to utilize your graphic design skills to consider color palettes, image contrast, text legibility, etc.

A good hero image requires an artistic touch.

I would suggest you mock-up your hero image in a program such as Illustrator first. Determine if you need to do any processing to the image to assist in its readability. Export the image from this program (not the text overlays). Use this image for your site, and use CSS to position the textual overlays. 
