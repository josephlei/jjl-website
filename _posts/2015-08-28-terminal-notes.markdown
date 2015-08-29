---
layout: post
title: "The VIM Way"
date: 2015-08-28
categories: 
published: true
---

###The VIM Way

####Decided to separate the one huge tips and tricks page into discrete topics

####**Updated 2015-08-22**

* `dd` deletes the line you're on
* `dG` deletes to end of file (EOF)
* `d$` deletes to end of line (EOL)
* `G` takes you to EOF
* `o` delta insert mode, nav down one line


* Placeholder for cmd/term/shell, to be moved to appropriate article
 * `ls -alt` list all, including hidden/dir, long format, ordered by mod datetime
* `ls | grep -i homebrew` to list using grep match, this is awesome
* cp m*.txt destination_dir
* cp * destination_dir
* `cat oceans.txt` displays contents of oceans.txt on stdout
* `cat a > b` REDIRECTS a on top of b, OVERWRITTING B
* `cat a >> b` APPENDS a behind b, keeping both
* `|` is a pipe, redirects left side to right side as stdin, i.e. "command to command redirection"
* `wc` command outputs lines, words, chars
* `sort lakes` sorts the contents of lakes and returns it, DOES NOT MOD ORIGINAL
* `cat lakes.txt | sort > sorted-lakes.txt` pipes the data to sort, output to sorted-lakes
* `uniq` cmd returns adjacent unduplicated version
* grep stands for "global regular expression print". It searches files for lines that match a pattern and returns the results. It is also case sensitive
 * grep -i enables case insensitive search
* `grep -R Arctic /home/` greps down a directory returning matches
* `sed` stands for stream editor, It accepts standard input and modifies it based on an expression, before displaying it as output data. It is similar to "find and replace".
* `'s/snow/rain/' forests.txt` searches forests.txt for the word snow and replaces it with rain, CAUTION: will only replace the first instance, g option on the end means "global" and match/replaces all instances!

