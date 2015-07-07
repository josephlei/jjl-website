---
layout: post
title: "Tips and Tricks picked up along the way"
date: 2015-06-13
categories: 
published: true
---

###A random collection of useful bits I want to remember as I learn

####(Also.. so I can erase it off ALL THE WHITEBOARDS)

####**Updated 2015-06-30**

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
* `None` is the python equivalent of Null (i.e. if x==None)?
* `scrapy version` displays version.. duh (no need for -- prefix)
* `~/.bash_profile` add `alias ll='ls -l'` for instant access to ls verbose (incl. permissions)
* `~/.bash_profile` add `export PATH="$PATH:~/scripts"` to add scripts dir to path, global .sh/any cmds
* on OSX, homebrew is used instead of apt-get
* `brew update` to update all libs, only exec via wifi, high dx xfer

* VIM `:q!` quits and discards changes
  * Ctrl + a Go to the beginning of the line (Home)
  * Ctrl + e Go to the End of the line (End)
  * Ctrl + p Previous command (Up arrow)
  * Ctrl + n Next command (Down arrow)
  * Alt + b Back (left) one word or use Option+Right-Arrow
  * Alt + f Forward (right) one word or use Option+Left-Arrow
  * Ctrl + f Forward one character (same as right arrow)
  * Ctrl + b Backward one character (same as left arrow)
  * Ctrl + xx Toggle between the start of line and current cursor position
  * Ctrl + l clear screen, does NOT clear buffer/history, simple equiv to `$clear`
  * Ctrl + U Clears the line before the cursor position. If you are at the end of the line, clears the entire line.
  * ctrl + H backspace
  * ctrl + D exit
* find out what xcode 11 cmd line tools is/means
* in Word, ^t is the find/replace for "tab", ^p for newline (ie. carriage return/Paragraph mark)