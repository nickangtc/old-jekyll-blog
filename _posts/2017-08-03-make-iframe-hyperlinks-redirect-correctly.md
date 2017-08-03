---
title: "Make iframe hyperlinks redirect in main document"
date: 2017-08-03T20:00:00+08:00
author: Nick Ang
layout: post
permalink: /make-iframe-hyperlinks-redirect-correctly/
categories:
  - technical
tags:
  - programming
  - html
---

At work recently we had to figure a way to redirect a user to another webpage when she clicks on a URL. This is obviously a trivial task for 99 percent of cases - just use `<a href="http://destination-url.com">Click</a>`. But within an `<iframe>`, URL redirects can act strangely.

<!--more-->

Let's say you're building a HTML/CSS/JS recommendation widget that is supposed to be embedded on people's e-commerce websites. When a user clicks on an image in the widget, you want to redirect her to the product detail page. But because your widget is actually embedded within an iframe (for ease of installation - UX!), when the user clicks on an image, she gets redirected to the product page _within_ the iframe, while the main window remains on the same page. That is unintended behaviour and it needs to be fixed.

Thankfully, the fix in this situation is very, very simple. Apparently there is a HTML element called [`<base>`][1] that handles this.

```html
<base target="_parent">
```

By adding this line of code in the `<head>` of your iframe, all URL redirects will happen on the parent document instead of in the iframe document. Something like this:

```html
<!doctype html>
<html>
<head>
  <link href="https://fonts.googleapis.com/css?family=Lato:300,700" rel="stylesheet">

  <!-- Force iframe URL clicks to open in main document -->
  <base target="_parent">

</head>
<!-- etc -->
</html>
```

I wish all web-related problems had beautiful, pre-emptive solutions like `<base>`!

[1]: https://developer.mozilla.org/en/docs/Web/HTML/Element/base
