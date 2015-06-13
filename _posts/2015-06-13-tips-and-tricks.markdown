---
layout: post
title: "Tips and Tricks picked up along the way"
date: 2015-06-13
categories: 
published: true
---

###A random collection of useful bits I want to remember as I learn
#### (Also.. so I can erase it off ALL THE WHITEBOARDS)

####**Updated 2015-06-13**

* `echo $PATH` gives you a colon separated list of your path environment (env) variable (var)
  * `echo $PATH > filename` will output your path env var to a file named filename, located in current working directory
  * in sublime or other text editor, use find replace to FIND all colons `:` and REPLACE with the regular expression for newline `\n` to make it readable

* To use a markdown bulleted list WITHIN another bulleted list, the syntax is EXACTLY as follows on a separate line following the "outer" bullet, periods are placeholders for spaces:

    `..*.enteryourtexthere` 

    (**READ**: `space` `space` `asterisk` `space` enteryourtexthere) YES it is very exacting
* Change permissions with `chmod 700 filename` using octal notation or permission +/-/= notation
* Rename a file by moving it within the same directory i.e. `cp file-x file-y` will rename file-x to file-y