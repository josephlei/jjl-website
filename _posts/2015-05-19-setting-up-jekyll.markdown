---
layout: post
title:  "Setting up Jekyll, the Good, the Bad and the Ugly"
date:   2015-05-19 11:44:00
categories: jekyll update
---
The chronicles of setting up this Jekyll built site with GitHub Pages.. some lessons learned:

1. _config.yml is dang important, baseurl parameter is what makes github serve it up the same way as localhost:4000
2. CNAME set up with a external domain sucks and takes time.. still waiting for DNS resolution, do this first so you can start the clock on the 24-48 hours it takes to update DNS @ records
3. YAML front matter is required on almost EVERYTHING
