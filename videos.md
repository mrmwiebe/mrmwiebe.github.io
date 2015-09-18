---
layout: display
title: Videos
permalink: /videos/
---

{% include header.html %}

<div id="video-thumbnails" class="container px2 py1">
    <div class="clearfix mxn2">

        {% for post in site.categories['homepage-video'] limit:12 %}

            {% include video-thumbnail.html %}

        {% endfor %}

    </div>
</div>
