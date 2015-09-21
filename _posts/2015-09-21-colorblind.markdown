---
layout: post
title: "How I beat being colorblind with wget/css"
date: 2015-09-21
categories: 
published: true
---

####**Updated 2015-09-21**

###The Backstory
I found out I was red/green colorblind sometime in elementary school and never thought much of it.  Being colorblind doesn't mean I can't see the color and totally miss out on things like Christmas; more so it means that I have a hard time telling the two apart when the hues are similar. Until recently, this "disability" didn't really affect me in any significant way except my friends asking me what color something was; I could/can see traffic lights just fine and so on.

###The Challenge
Recently, in my quest for data domination I have made it a goal to learn VIM (a command line text editor) and Regular Expressions (A way of matching string patterns).  In the course of learning regex in particular, I came across a website with great tutorials and was a great way to learn.. **except** the main colors used were, you guessed it.. red, green and blue. 

[Check out this link to see the page in question](http://www.regular-expressions.info/quickstart.html)

###The Solution
For a couple months I tried to find alternate sites and learning material but it bothered me that this common color scheme could genuinely affect my ability to learn.  One day I ran into my friend Gary L. at the Sacramento Hacker Lab and he suggested using browser code injection tools like tampermonkey css to modify the local cached version of the website so I could see the colors.  Ultimately if I followed his suggestion, the end result might be even more elegant than what I finally landed on, but would allow me to not divert energy learning a new language. 

Since I had been fiddling with command line wget for a while, I used this as an opportunity to road test what I had picked up so far.  

**The Goal:**
  1. Clone the entire website excluding links to external websites
  2. Modify the local cascading style sheet to colors I can see

What I landed on was the following: `wget --limit-rate=200k --no-clobber --convert-links --random-wait --domain=regular-expressions.info -r -p -E -e robots=off -U mozilla http://www.regular-expressions.info/`

When all the smoke had cleared, I was 3.4 MB heavier and halfway to the goal 

`Total wall clock time: 19s`

`Downloaded: 160 files, 3.4M in 2.1s (1.65 MB/s)`

I then modified the .css to make the colors distinctly different by changing the red into bright YELLOW and the green into a distinctly uh.. GREEN green.

###The Result

Below are two pictures showing the before and after, markedly different.  The best part about this solution is that **IT AUTOMATICALLY AFFECTS EVERY LOCALLY CACHED PAGE** which means I can now learn to my hearts content, colors and all.

####I hope this article has been fun and that it will be helpful for others who have the same issue with colors. If you know any color "challenged" people, please feel free to share this with them :)
`:wq`

###**BEFORE**
![before](/assets/colorblind_before.png)
###**AFTER**
![after](/assets/colorblind_after.png)
