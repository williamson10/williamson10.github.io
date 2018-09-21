---
layout: page
title: About me
techused:
  - windows
  - linux
  - bananas
---
I have always been drawn to computers. As a teen in the 90's, computers were the future and I was hand typing QBASIC code from a book to see if it would run. This was fun for me and I still have that curiosity and dry sense of a good time. In my travels I have dabbled in a lot of things. I've played with [PowerShell](https://github.com/williamson10/PowerShell), [Python](https://github.com/williamson10/pyGridWars), [git](https://github.com/williamson10), [Jekyll](https://github.com/williamson10/williamson10.github.io/), and others. (See below for an exhaustive list) I want this site and OpenLAB to be the culmination of all that experimentation. 

### Technologies Used
{% for tech in page.techused %}
  *{{ tech }}
{% endfor %}
