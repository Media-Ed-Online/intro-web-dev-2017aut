---
title: Review the Head Element
module: 6
---

# Review the Head Element

Now that we are wrapping up our section on HTML, lets review the basic structure of the document and the elements that should populate the HTML page's head element.

## Above `<head>`

As a reminder, the first line in your document should be a doctype declaration, in most cases, this should specify that the document is in HTML5.

```html
<!DOCTYPE html>
```

## `<html>`

The next line in your document should be the opening `<html lang="en">` tag along with the ISO language code.

## `<head>`

Following these, should be the `<head>` element. This should contain at a minimum a;

- `<title>...</title>`
- `<meta charset="utf-8">`
- `<meta name="author" content="">`
- `<meta name="description" content="">`


## All Together Now

So the basic structure of your document along with metadata should look something like...

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta name="author" content="Michael Musick">
    <meta name="description" content="A Basic HTML Template">
    <title>Your Site's Title</title>
  </head>
  <body>
    <!-- content -->
  </body>
</html>
```
