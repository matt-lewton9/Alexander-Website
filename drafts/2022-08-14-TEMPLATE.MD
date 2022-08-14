layout: post
title: TITLE HERE
excerpt_separator: <!--more-->
image: assets/images/FILENAME.jpeg
---

This is a paragraph of text in the excerpt before the first seperator, I can't have any images in the excerpt.

The name of this file must be formatted YYYY-MM-DD-TitleName.md

<!--more-->

This is no longer in the excerpt, let me add an image.

{% include image.html file="FILENAME.jpeg" caption="This is the image caption" maxWidth = "250px" %}

file is the name of the image file in assets/images, the caption is text that is displayed below the image, and width is the max width of the image in pixels.

Sometimes, you'll want to display 2+ images at once, and the current format will be gross. So, put images within a div using the html formating below.

<div style="display:flex; justify-content:center; align-items:center; flex-wrap:wrap;">

{% include image.html file="FILENAME.jpeg" caption="This is the image caption" maxWidth = "250px" %}

{% include image.html file="FILENAME.jpeg" caption="This is the image caption" maxWidth = "250px" %}

{% include image.html file="FILENAME.jpeg" caption="This is the image caption" maxWidth = "250px" %}

{% include image.html file="FILENAME.jpeg" caption="This is the image caption" maxWidth = "250px" %}

</div>

That box will display 4 images. It's important that the ending div marker is there.

Lastly, say that you wanted to insert a link to a significantly cooler website, that would look like {% include url.html url="https://mattlewton.me/" text="this" %}.

where url is the url of the site, and text is the text that will be displayed
