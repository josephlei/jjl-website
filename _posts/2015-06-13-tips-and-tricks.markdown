---
layout: post
title: "Tips and Tricks picked up along the way"
date: 2015-06-13
categories: 
published: true
---

###A random collection of useful bits I want to remember as I learn

####(Also.. so I can erase it off ALL THE WHITEBOARDS)

####**Updated 2015-08-22**

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
* Markdown headings must be separated by a new line, otherwise the 2nd heading markdown won't take effect
* Explore CURL/GREP/WGET
  * ex: wget http://www.regular-expressions.info -r -l 2 (recursive, depth of TWO)

* `pip install -r requirements.txt` installs the packages specified in requirements.txt, -r flag necessary
* `pip freeze > stable-req.txt` dumps out the current library env to a file named stable-req.txt
* `scrapy version` displays version.. duh (no need for -- prefix)
* on OSX, homebrew is used instead of apt-get
* `brew update` to update all libs, only exec via wifi, high dx xfer
* find out what xcode 11 cmd line tools is/means
* in Word, ^t is the find/replace for "tab", ^p for newline (ie. carriage return/Paragraph mark)

* Virtualenv + Condaenv
  * `$source bin/activate` in a virtualenv to activate it, `$deactivate` to deactivate

* Python via Codecademy
  * `None` is the python equivalent of Null (i.e. if x==None)
  * use backslash to escape quotes in a string, i.e. 'This isn\'t going to cause a problem'
  * str methods, len() lower() upper() str()
  * methods that use dot notation such as lion.upper() only work with STRINGS
  * `\` is the continuation character, use cases?
  * raw_input("interrogative") from console (stdin) unless def. differently
  * not > and > or (order of operations without parens)
  * x.isalpha() checks if only a-z in str
  * `import math` is an example of a generic import, brings in all functions and definitions, requires prefix of library before functions i.e. `math.sqrt(25)`
  * `from module import function` imports just the one function, it is called a "function import" example `from math import sqrt` now you can just type print sqrt(25)
  * universal import `from math import *`
  * dir(math) contains everything that was imported
  * del dictionary['key'] will delete the KVP
  * LISTS have a remove method via list.remove(item)
  * "".join(list) joins the elements together with dlm within ""
  * removing from lists, n.pop(1) removes/returns the item at index 1, n.remove(1) removes the item with VALUE "1" if it finds it, del(n[1]) deleted item at index 1, doesn't return you anything
  * range(stop), range(start, stop), range(start, stop, step) is a generator, creates a list up to but EXCLUDING stop, def start =0, step=1
  * `break` takes you out of the current loop, not an entire function
  * while/else construct, else will run when while becomes false or never runs, will NOT run if it is a result of a break keyword
  * anonymous functions, anon f(x)s allow "functional programming", can pass functions around as if they were vars or vals.  i.e. no name functions
   * lambda x:x%3==0 is the same as def by_three(x): return x%3==0
  * function bin(x) returns the binary equivalent of x, oct(x) and hex(x) for base 8 and 16
  * int function has an optional 2nd argument int(string containing number, base), example int("111") or int("0b100",2)
  * right and left bit shifts are the equivalent of floor dividing and multiplying by 2, or shifting all the 1s and 0s to the right or left by the given number, can only be performed on an integer, all others will give gibberish
  * class scope global var vs. member vars (only to members of a certain class), instance var only avail to particular instances of a class

* Term/shell
  * `!!` gives you the last entered COMMAND, `sudo !!` to root last w/o re-typing
  * `!$` gives you the last entered ARGUMENT (test with `$echo !$`)
  * `open .` opens the current working directory in finder, replace `.` with filename to open w/linked def app
  * `~/.bash_profile` add `alias ll='ls -l'` for instant access to ls verbose (incl. permissions)
  * `~/.bash_profile` add `export PATH="$PATH:~/scripts"` to add scripts dir to path, global .sh/any cmds
  * `$history` for prev commands, then use `!###` to execute
  * `cd -` to toggle between last two active dirs
  * Rename a file by "copying" it within the same directory i.e. `cp file-x file-y` will rename file-x to file-y
  * UBUNTU
    * `sudo dpkg-reconfigure tzdata` to update time zone, may have to restart cron/others with `restart cron`
  * `uname -r` to get kernel version
  * To remove password from .ssh key use `ssh-keygen -p`
  * `which wget` to check where it is
  * `lsb_release -a` to check ubuntu + codename i.e. trusty, precise pangolin, etc.
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
  * `find . -name 'Screen Shot*' -exec mv -i {} ~/Desktop/Screen\ Shots \;` moves all screen shots on desktop to folder indicated

  * `$ defaults write com.apple.screencapture location /drag/location/here` followed by `$ killall SystemUIServer` to change ss directory

* Regex
  * `\n` is for newline
  * `<.*>` to select inside tags

* Docker
  * `sudo docker -d &` to start the docker daemon if it is not already running
  * `sudo docker` to see a list of all commands
  * `sudo docker info`
  * `sudo docker version`
  * `sudo docker search ubuntu` example to search for images
  * `sudo docker pull ubuntu`
  * `sudo docker images`
  * `sudo docker commit [container ID] [image name]` example below
    * `sudo docker commit 8dbd9e392a96 my_img`
  * `sudo docker push [username/image name]` example below
    * `sudo docker push my_username/my_first_image`
  * `sudo docker ps` to list all running containers
    * `sudo docker ps -l` to list both running and non-running
  * index.docker.io is the hub (i.e. hub.docker.com) j.l@gmail.com login auto pass