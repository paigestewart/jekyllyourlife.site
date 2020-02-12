---
layout: post
title: Create a new Jekyll site
date: 2020-02-11 15:54 -0700
---
# First, you must install the environment
Jekyll requires Ruby, Git Bash and some other software. Check [here](https://jekyllrb.com/docs/installation/) to see what you need. You'll also need an account at [GitHub](https://github.com/).

*Be sure to check the installation guides for your Windows, Mac or Linux system.*

*Be sure to note where you've installed Ruby - you'll likely be searching for and working with those files later*

*Note that you'll also need a text editor like Atom, Visual Basic, etc.*

# Once you've finished installing what you need
Open your terminal:

`Cd` navigate to wherever you want the site files to live - eg): `cd documents`

`Jekyll new siteName` to create a new Jekyll site - siteName refers to whatever you want the folder to be called

`Cd` navigate to the new Jekyll instance - eg): `cd siteName`

`Atom .` to open it up in Atom or another text editor - *note the space between Atom and .*

And there you have it - a new Jekyll site!

# You'll also need to make your Jekyll site into a git repository

Open your terminal:

`Git init` to initialize the git repository

`Git status` to see all the files you've created or changed

`Git add --all` or you can name specific files

`Git commit -m “note on the commit”` for your first commit, you might want to write "first commit" or whatever else you've edited

`Bundle lock --add-patform ruby` this piece will link the repo (repository) to ruby

`Bundle lock --add-platform x86_64-linux` another necessary linking piece

# And Voila!
In your terminal, `bundle exec jekyll serve` will start up your new site on a preview server, likely localhost:4000 in your browser, and
holding CTRL or CMD + C will stop the preview server

[Back to home]({% link index.markdown %})
