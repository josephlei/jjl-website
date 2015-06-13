---
layout: post
title: "Tips and Tricks I've picked up along the way"
date: 2015-06-13
categories: 
published: true
---

###A random collection of useful bits I want to remember as I learn

####**Updated 2015-06-13**

* echo $PATH gives you a colon separated list of your path environment (env) variable (var)
  * echo $PATH > filename will output your path env var to a file named filename, located in current working directory
  * in sublime or other text editor, use find replace to FIND all colons `:` and REPLACE with the regular expression for newline (\n) to make it readable
* To use a markdown bulleted list WITHIN another bulleted list, the syntax is EXACTLY as follows on a separate line following the "outer" bullet, replace periods with SPACES: "..*.texthere" YES it is very exacting, will post it more clearly with inline code quotes soon