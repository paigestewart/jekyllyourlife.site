---
layout: post
title: Create a new Jekyll site
date: 2020-02-11 15:54 -0700
---
## First, you must install the environment. Jekyll requires Ruby, Git Bash and some other software. Check [here](https://jekyllrb.com/docs/installation/) to see how to begin the installation process.

# You'll also need an account at [GitHub](https://github.com/).

*Be sure to check the installation guides for your Windows, Mac or Linux system.*

*Be sure to note where you've installed Ruby - you'll likely be searching for and working with those files later.*

*Note that you'll also need a text editor like Atom, Visual Basic, etc. I recommend Atom, which can be installed from [here](https://atom.io/), but Jekyll also recommends a few [here](https://jekyllrb.com/resources/) under editors.*

# Once you've finished installing what you need

Open your terminal:

`Cd` navigate to wherever you want the site files to live - eg): `cd documents`

`Jekyll new siteName` to create a new Jekyll site - siteName refers to whatever you want the folder to be called

`Cd` navigate to the new Jekyll instance - eg): `cd siteName`

`Atom .` to open it up in Atom or another text editor - *note the space between Atom and .*

And there you have it - a new Jekyll site!

# You'll also need to make your Jekyll site into a git repository (so you can control versions and upload it to GitHub later. The site will be hosted on GitHub!)

Open your terminal:

`Git init` to initialize the git repository

`Git status` to see all the files you've created or changed

`Git add --all` or you can name specific files

`Git commit -m “note on the commit”` for your first commit, you might want to write "first commit" or whatever else you've edited

`Bundle lock --add-patform ruby` this piece will link the repo (repository) to ruby

`Bundle lock --add-platform x86_64-linux` another necessary linking piece

# A couple extras

**In your gemfile,** install this plugin: `‘jekyll-compose’, group: [:jekyll_plugins]` so you'll be able to post easily and correctly from the command line. Run `bundle` in the command line.

`bundle exec jekyll post "postTitle"` is the command to post. Try it! Make a post called "FirstPost"!

**In your config.yml file,** add a line reading `destination: public`, then add `public` to your gitignore file - this will put all your site files into one folder for deployment, but won't add them to your public GitHub repository when the time comes.

# And Voila!
In your terminal, `bundle exec jekyll serve` will start up your new site on a preview server, likely localhost:4000 in your browser, and
holding CTRL or CMD + C will stop the preview server. Note that changes to your config.yml file won't work if your preview server is running. Otherwise, though, all the changes you make will show up in your preview server if you press refresh!


[Back to home]({% link index.markdown %})
