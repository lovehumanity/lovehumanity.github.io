---
title: "Creating a Blog for Free"
date: 2020-11-03
classes: wide
categories:
  - Productivity
header:
  teaser: "/assets/blogs/2020-11-03-Creating-a-free-blog/blog.jpeg"
---

This guide will look at how to use jekyll to create your own static blog hosted completely free using either GitLab or GitHub. This guide will use Arch Linux as the system, although others distros will have a similar install procedure.

First start by installing ruby on your system

Arch:
```
sudo pacman -S ruby
```

Debian 
```
sudo apt-get install ruby ruby-dev
```

Next you need to prepend the ruby path into your path variable
add this to your ~/.profile
PATH="$PATH:$(ruby -e 'puts Gem.user_dir')/bin"
or you can execute this in terminal and it will change your PATH variable until the next reboot
see https://wiki.archlinux.org/index.php/Ruby

After install jekyll and bundler with

```
gem install jekyll bundler
```

Next you can look in jekyll for a theme that you like
http://jekyllthemes.org/

In this guide I will be using Minimal mistakes, but the installation will be similar for other themes 

Next you will need the theme you can either download the file in releases or do a git clone

```
git clone https://github.com/mmistakes/minimal-mistakes
cd minimal-mistakes
bundle install
```

Next to confirm that it is working as expected you can serve the blog locally using 
```
bundle exec jekyll serve
```

And you should be able to visit the website under http://127.0.0.1:4000

You then run this same command from within the main directory to view your posts locally before publishing them

## Creating posts

Create a directory in the root dir \_posts 
```
mkdir \_posts 
mkdir \_posts/2020
```

the basic format for file names is 2020-08-21-new-blog.md

## Some Basic Configurations 

For this blog I wanted the navigation bar to have some other pages so I changed \_data/navigation.yml with 
\# main links
main:
   - title: "About"
     url: /About 
   - title: "Contact"
     url: /Contact

Next I made a directory in the root dir \_pages and made the files about.md and contact.md

In both there contents I used the format

---
title:  "Contact"
layout: archive
permalink: /Contact/
---

Check out the official documentation, the way you want it configured is likely there, you can also look at the sample blog that it has and look at the source files for them on their github page

https://mmistakes.github.io/minimal-mistakes/year-archive/
https://github.com/mmistakes/minimal-mistakes/tree/master/docs


## Other Stuff

I didn't want to share links on the blog so needed to edit ~.config.yml
and edit 
defaults
share: false

I also didn't want to show a profile on the home page so edited 
author\_profile: false
in .config.yml

Also edit .config.yml title,description 

To edit the default size of the font you can change the file /_saas/minimal-mistakes/_reset.scss and edit the pixel sizes. See [this](https://github.com/mmistakes/minimal-mistakes/issues/1219) and [this](https://github.com/mmistakes/minimal-mistakes/issues/1184)

## Publishing 

So after you have the blog setup in the way that you want you can publish it for free on GitHub/GitLab as they both allow for free hosting of static content.

I will show how to publish in GitLab.

First create a repository in GitLab and name it USERNAME.gitlab.io where USERNAME is the username of your GitLab account. 

Next you need to push the files that you have on your local computer to that GitLab repository 
but before you do that you need to initialise a git repo in that folder, so go into the folder with your template and rename it to be USERNAME.gitlab.io where USERNAME is your GitLab username. Then run
git init 
which will initialise the git repos on in that folder
if you haven't done so already you need to add an email address and a name for git to do this run
```
git config --global user.email \<Your email\>
git config --global user.name "\<Your name\>
```

```
git add --all
git commit -m "Initial commit of Jekyll blog"
```

Then you need to set the origin 
```
git remote add origin https://gitlab.com/lovehumanity/lovehumanity.gitlab.io.git
```
If you get the remote origin wrong you can change it using 
```
git remote set-url origin https://gitlab.com/lovehumanity/lovehumanity.gitlab.io.git
```


For whatever reason the GitLab repo was different to my local repo so if you run in to the same issue you can just use git pull to ensure that you don't have any errors of the GitLab repo having extra files than your local repo 
```
git pull origin master
```
and this should ensure that your local repo is the same as your GitLab repo

After that you need to now create a new file in that repository and have that file be a \_gitlab\_config.xml and choose the jekyll template. Once that has been added GitLab should automatically start building your static website. To check look at pipelines and you should see it running/completed there  

After the runner has completed you should be able to visit USERNAME.gitlab.io and see your newly created website. If you don't see your new website, it may be that you need to change permissions of the repository to be public. 

To do that goto the repository's settings and it should give you the option to change it to public.


To make changes, you can make the changes locally and then use git to apply those changes to your GitLab repo using.
```
git add .
git push origin master
git commit -m "Second post published"
git push origin master
```

