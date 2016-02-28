---
layout:     post
title:      Ionic Video Link
date:       2015-12-08
categories: blog webdev code
---

Before making trailers fulltime, I made HTML things.  One of these things is a special video tag for the speedy hybrid app framework called [Ionic](getsoundmind.com).

I was making an app for a company in Winnipeg called [Soundmind Health Technologies](ionicframework.com).  In this particular app, I needed to be able to show a list of videos and when they were clicked, smoothly animate and fade into the video and have them start automatically.  

So, I thought that this would be the best time to try out one of [Angular's directives][5464de04], which basically lets you make up your own HTML tags and wrap them with custom javascript and behaviors.  Very cool, but can be tricky to get your mind around how it all works.

  [5464de04]: https://docs.angularjs.org/guide/directive "Angular Directives"

Anyways, I made a directive that makes links and auto loads videos when you click them.  Here's what it looks like in action:

<div class="col-12 center">
 <img src="/images/posts/2015/ionic-video-link.gif" style="border:1px solid grey"/>
</div>

Here's a sample of what I used for the list above:

```html
<ionic-video-link video-src="assets/Getting Started.mp4" video-name="getting-started">
    <ion-item>
        <i class="icon ion-ios-play-outline"></i>
        &nbsp;Getting Started
    </ion-item>
</ionic-video-link>
```

The directive preserves whatever you have inside the ionic-video-link tag so you can use it for any sort of link!  Very handy.

That's it!  The directive takes care of the rest.  Check out the [GitHub repo][1dbb0547] and send me any bugs or any questions you may have. :)

  [1dbb0547]: https://github.com/mrmwiebe/ionic-video-link "Ionic Video Link GitHub Repo"

Cheers!
