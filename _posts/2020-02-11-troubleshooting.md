---
layout: post
title: Troubleshooting
date: 2020-02-11 14:18 -0700
---

# General troubleshooting go-to:

* Copy/paste the error the terminal is reporting into google and see what people are saying
* [Jekyll Docs Troubleshooting](https://jekyllrb.com/docs/troubleshooting/)

# Some issues we encountered:

**Terminal reports gems or themes cannot be found after installing theme gem:**

* You may need to move the mentioned files into the library of gems inside your ruby software files. Sometimes gems don't go into the right spot, or you downloaded them outside the terminal onto your desktop, for example. For this fix you'll need to find your ruby files, then dive into ruby/lib/ruby/gems/2.6.0/gems, and move the right theme files into the right spot.
* Replace theme name in config.yml and gem "theme-name" in gemfile

**Terminal reports that it can’t find theme files after editing things in layouts/css/scss and attempting to build the site:**

1. Make sure you're in the right folder! If your actual folder is called JekyllSite but you're in jekyllsite, the system may get confused.
1. Reinstall the theme gem you're working with eg): `gem install jekyll-theme-athena`
2. Rename ‘destination’ in config.yml and delete old destination folder (public)
3. Try `bundle exec jekyll serve` again

Reminder:

In config.yml:
`Destination: public`

In gitignore:
`Public` (so that we don’t push our public site files into git)

*Note that you do not have to name the destination folder "public", you can name it anything you'd like.*

**Generally, empty your baseurl/url tags in config.yml - if they contain anything (while you're editing) you may encounter errors.**

**When a theme requires a different version of Jekyll**
* Downgrading Jekyll to previous versions is necessary for some themes
1. Find and replace the Jekyll version with the necessary Jekyll version (the terminal will tell you which) in your gemfile, then `Bundle update jekyll`
2. You may also need to `Bundle update` and/or `bundle install` depending on the issue
3. You may also need to delete the gemfile *.lock* (**note: NOT the gemfile**) and try these steps again

[Back to home]({% link index.markdown %})
