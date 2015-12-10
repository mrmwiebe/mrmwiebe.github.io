---
layout:     post
title:      Ionic Video Link
date:       2015-12-08
categories: blog webdev code
---

I don't do much webdev anymore, other than on this site, but one of the last web development things that I have been working on before doing trailers fulltime was making an app for a company in Winnipeg called [Soundmind Health Technologies][3c479271].  I had extensive knowledge in HTML and had convinced them to make it using the [Ionic Framework][f1629ad0] which is a HTML5, cross-platform, speedy library for making hybrid apps.  It's a great framework, definitely the speediest one that I've seen, but still has it's quirks.

  [f1629ad0]: ionicframework.com "Ionic Framework Homepage"
  [3c479271]: getsoundmind.com "Soundmind Homepage"

In this particular app, I needed to be able to show a list of videos and when they were clicked, smoothly animate and fade into the video and have them start automatically.  So, I thought that this would be the best time to try out one of [Angular's directives][5464de04], which basically lets you make up your own HTML tags and wrap them with custom javascript and behaviors.  Very cool, but can be tricky to get your mind around how it all works.

  [5464de04]: https://docs.angularjs.org/guide/directive "Angular Directives"

Anyways, I made a directive that makes links and auto loads videos when you click them.  Here's what it looks like in action:

<img src="/images/posts/2015/ionic-video-link.gif" alt="" style="align:center;" />

Here's a sample of what I used for the list above:

'''html
<ionic-video-link video-src="assets/Getting Started.mp4" video-name="getting-started">
    <ion-item>
        <i class="icon ion-ios-play-outline"></i>
        &nbsp;Getting Started
    </ion-item>
</ionic-video-link>
'''

The directive preserves whatever you have inside the ionic-video-link tag so you can use it for any sort of link!  Very handy.

That's it!  The directive takes care of the rest.  Check out the [GitHub repo][1dbb0547] and send me any bugs or any questions you may have. :)

  [1dbb0547]: https://github.com/mrmwiebe/ionic-video-link "Ionic Video Link GitHub Repo"

Cheers!
