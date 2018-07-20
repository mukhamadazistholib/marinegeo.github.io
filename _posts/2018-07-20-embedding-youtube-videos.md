---
layout: post
title: How To Embed Videos
subtitle: Add Youtube Videos with an iframe
tags: [help, website]
---

## `<iframes>`

In order to add a video to a module page, we will need to use an HTML element called an `<iframe>` to the markdown page. Jekyll can understand a mix of HTML and markdown.
An `<iframe>` is an element that allows an external webpage to be embedded in an HTML document.
For example, to add a tutorial video from Youtube...
```HTML
<!-- iframe of youtube video with set height & width -->
<iframe src="https://www.youtube.com/embed/GP8c24aNykg" frameborder="0"
      allowfullscreen width="560" height="315" ></iframe>
```
<br>
<iframe width="560" height="315" src="https://www.youtube.com/embed/GP8c24aNykg" frameborder="0" allowfullscreen></iframe>

## Responsive Layout

To make the embedded video automatically fit the page layout, wrap the iframe in
a [Bootstrap responsive embed class](https://getbootstrap.com/docs/3.3/components/#responsive-embed).

```html
<!-- 16:9 aspect ratio -->
<div class="embed-responsive embed-responsive-16by9">
  <iframe class="embed-responsive-item" src="..."></iframe>
</div>

<!-- 4:3 aspect ratio -->
<div class="embed-responsive embed-responsive-4by3">
  <iframe class="embed-responsive-item" src="..."></iframe>
</div>
```
<br>
<div class="embed-responsive embed-responsive-16by9">
  <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/GP8c24aNykg"></iframe>
</div>
