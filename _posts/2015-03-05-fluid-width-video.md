---
layout: post
title:  "Fluid width video"
date:   2015-03-05 14:53:10
categories: code
tags: css
---

Ok this code will make your video (iframe) will flow like a fluid. This code I got from somewhere, I forgot the link.

**html :**  
{% highlight html %}
<div class="videoWrapper">
    <iframe width="420" height="315" src="https://www.youtube.com/embed/C7pP1csDBD4" frameborder="0" allowfullscreen></iframe>
</div>
{% endhighlight %}


**css**  
{% highlight css %}
videoWrapper {
	position: relative;
	padding-bottom: 56.25%; /* 16:9 */
	padding-top: 25px;
	height: 0;
}
.videoWrapper iframe {
	position: absolute;
	top: 0;
	left: 0;
	width: 100%;
	height: 100%;
}
{% endhighlight %}