---
layout: post
title: First Post
subtitle: An Introduction and Intent
tags: [Intro]
---

Hi there, my name is Justin. If you are reading this you are probably checking up on me and if you've come this far, maybe your willing to come a little further. You remember the name of the town don't you?

Shawshank aside, on this site you will find write ups and ramblings from my technology adventures. My goal is to share some of the knowledge that I have amassed over the years as well as showcase my abilities that my employment past does not show. This site being the first project.

This site was created using the static site generator, [Jekyll](https://jekyllrb.com/). It does use a theme called [beautiful-jekyll](https://github.com/daattali/beautiful-jekyll) although I have made a few modifications to make it my own. You can see all the changes on my [Github](https://github.com/williamson10/williamson10.github.io). In fact this site is hosted for free on [Github Pages](https://pages.github.com/).

For development of this site, I chose to develop locally and push the changes to github. I find it much faster plus it required me to spend more time with git and that is always a good thing. If you look at the commit history, you would see where I had to commit every change when using the editor on Github and when I started locally and was able to make more sense of each commit.

![alt text](/img/2019-04-11/commits.png "Commits")

 The thing I struggled with was maintaining changes that made sense together versus just moving on to something else when I got frustrated. For example, I struggled a bit using the config variables in _config.yml to change the navbar color. After fighting with it and failing, I moved on to something else. When I went to commit those changes, I realized I still had some of the navbar changes that would have been part of the commit. I ended up reverting those changes, creating the commit, and then reverting the revert. It was messy. As I write this, I realized maybe I could have only staged the changes I wanted. More research to do.

For those curious about the navbar color issue, it ended up that I needed to delete the _site folder and let everything rebuild. This seems to be the case when changing any of the color variables in the config.yml.