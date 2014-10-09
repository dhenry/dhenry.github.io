---
layout: post
title: "It's alive!"
date: 2014-10-08 20:04:59 -0700
comments: true
categories: 
---
### Setting up a Github pages blog with Octopress

Install [git](http://git-scm.com/)

Create a [github account](https://github.com) if you don't have one.

Follow the [instructions](https://pages.github.com/) provided by github to
create a new repository that will automagically turn into a jekyll instance.

Open cygwin/powershell/command prompt and check your ruby version. `ruby -v`. 

Got `ruby 1.9.3`? You're set.

No ruby? [Install](http://rubyinstaller.org/downloads/) it then. 

Some other ruby version? [Install](http://rubyinstaller.org/downloads/) `ruby 1.9.3` and update your path 
variable to point to it. This will save you some headaches with gem compatibility 
issues.

Follow the instructions [here](http://octopress.org/docs/setup/) to setup Octopress.

Follow the instructions [here](http://octopress.org/docs/deploying/github/) to hook up your 
recently created github repository with the default octopress installation.

### Creating posts

If you haven't done so already, try `rake preview` and hit http://localhost:4000 to 
see your blog running locally.

Not much to see yet, huh...

To create a new post do a `rake new_post["Exciting new post"]`.

This will generate a .markdown file placed here: `octopress\source\_posts`

Jekyll watches for changes to files within the source directory so any changes you make
are visible after a browser refresh.

For tips on editing the .markdown files check out these [instructions](http://daringfireball.net/projects/markdown/syntax).

Once you're happy with your changes then commit and push to publish your content to Github pages.