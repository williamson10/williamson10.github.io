---
layout: post
title: Code Server with Jekyll
subtitle: Web IDE for my Chromebook
tags: [jekyll, code-server, docker,]
---

Straight to the point, I love my Chromebook. It's light, silent, and the battery lasts all day. For the most part it fits my needs. One of the major struggle points I had with it was a decent development environment. I know that ChromeOS now supports Linux apps as well as android but in my use of it, there were still a lot of road blocks. Mainly because of my ARM processor.  

About a month ago I read an article about [code-server](https://github.com/cdr/code-server) which puts Microsoft's excellent VSCode in a browser and it seemed like the perfect solution. I have been learning the ins and outs of docker recently as well so I decided to install their docker container. It works very well. 

Again the main issue I had for my Chromebook was the ARM processor. I could not find a way to get Jekyll running which meant I was not able to develop this site locally. Boo. Problem 2 was that code-server did not have Jekyll installed either so that wouldn't work. I decided to roll up my sleeves and try my hand at creating a docker image. 

I [forked](https://github.com/williamson10/code-server-jekyll) code-server, edited the dockerfile and uploaded it to [docker hub](https://hub.docker.com/r/williamson10/code-server-jekyll). This works great. The one issue I have is that after a fresh provision, I need to run `bundle install` in a terminal once. I assume this is because my project files are not available to the container at build-time. I mount my project folder as a directory at run-time.

I now have a browser based version of VSCode, able to serve and generate Jekyll sites and keep it all in sync with github. Life is great.

![alt text](/img/2019-04-27/code-server.png "CodeServer with Jekyll")

As I have also been playing with Terraform, [here](https://raw.githubusercontent.com/williamson10/terraform-docker-lab/master/code-server-jekyll.tf) is a bonus .tf file that will provision this for you. Bring your own docker provider config :)
