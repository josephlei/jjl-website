---
layout: post
title: "Tips and Tricks picked up along the way"
date: 2015-06-13
categories: 
published: true
---

###A random collection of useful bits I want to remember as I learn

####(Also.. so I can erase it off ALL THE WHITEBOARDS)

####**Updated 2015-06-15**

* `echo $PATH` gives you a colon separated list of your path environment (env) variable (var)
  * `echo $PATH > filename` will output your path env var to a file named filename, located in current working directory
  * in sublime or other text editor, use find replace to FIND all colons `:` and REPLACE with the regular expression for newline `\n` to make it readable

* To use a markdown bulleted list WITHIN another bulleted list, the syntax is EXACTLY as follows on a separate line following the "outer" bullet, periods are placeholders for spaces:

    `..*.enteryourtexthere` 

    (**READ**: `space` `space` `asterisk` `space` enteryourtexthere) YES it is very exacting
* Change permissions with `chmod 700 filename` using octal notation or permission +/-/= notation
  * READ = 4
  * WRITE = 2
  * EXEC = 1
  * NOTHING = 0
  * +/-/= (examples coming soon)
  * Explore recursive opt via -r/-R?
  * User/Group/Other? TBD will change
  * Use `ls -l<d> file/dir` to list with permissions
* Rename a file by moving it within the same directory i.e. `cp file-x file-y` will rename file-x to file-y
* Markdown headings must be separated by a new line, otherwise the 2nd heading markdown won't take effect
* Explore CURL/GREP/WGET
  * ex: wget http://www.regular-expressions.info -r -l 2 (recursive, depth of TWO)
* `$history` for prev commands, then use `!###` to execute
* `!!` gives you the last entered COMMAND
* `!$` gives you the last entered ARGUMENT (test with `$echo !$`)
* `open .` opens the current working directory in finder
* `pip install -r requirements.txt` installs the packages specified in requirements.txt, -r flag necessary
* `pip freeze > stable-req.txt` dumps out the current library env to a file named stable-req.txt
* `$source bin/activate` in a virtualenv to activate it, `$deactivate` to deactivate
* `cd -` to toggle between last two active dirs