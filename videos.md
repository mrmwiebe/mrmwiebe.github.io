---
layout: display
title: Videos
permalink: /videos/
---

{% include header.html %}

<div id="video-thumbnails" class="container px2 py1">
    <div class="clearfix mxn2">

        {% for post in site.categories['video'] limit:24 %}

            <div class="sm-col sm-col-4">
                {% include video-thumbnail.html %}
            </div>

        {% endfor %}

    </div>
</div>
