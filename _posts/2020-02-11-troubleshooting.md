---
layout: post
title: Troubleshooting
date: 2020-02-11 14:18 -0700
---
**When pushing your site to GitHub:**

If you get `Fatal error - origin already exists`, then run `Git remote rm origin`, then try `git push -u origin` again. You may also have to delete your repo (**not** your site) and start again.

**If gems or themes cannot be found:**
* You may need to move the mentioned files into the library of gems inside your ruby software files. Sometimes gems don't go into the right spot, or you downloaded them outside the terminal. For this fix you'll need to find your ruby files, then dive into ruby/lib/ruby/gems/2.6.0/gems, and move the right files in.
* Replace theme name in config.yml and gem ‘theme-name’ in gemfile

**Terminal reports that it can’t find files after editing things in the layouts/css/scss:**
* Reinstall and the theme gem you're working with
* Rename ‘destination’ folder and delete old one
* Try `bundle exec jekyll build again`

Reminder:

In config.yml:
`Destination: public`

In gitignore:
`Public` (so that we don’t push our public site files into git)

**When editing your site locally, get rid of baseurl/url in config.yml**

**When a theme requires a different version of Jekyll**
* Downgrade Jekyll to previous versions for some themes (find and replace the Jekyll version in config.yml file), then `Bundle update jekyll`
* You may also need `Bundle update` or `bundle install` depending on the issue

**General Troubleshooting Strategies**

* Copy/paste the error the terminal is reporting into google and see what people are saying
