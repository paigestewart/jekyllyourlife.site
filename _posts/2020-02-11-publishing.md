---
layout: post
title: Automatic Publishing
date: 2020-02-11 15:45 -0700
---
# When you're ready to publish, follow the following steps.
Don't worry if your site isn't totally finished. This process sets you up for automatic updates, so your site will update as you go.

**Start at step 1 if you've installed a theme gem. If you've cloned a theme repository, skip steps 2-5**

1. In your terminal while `cd` inside your site files, run `bundle exec jekyll build`  
  * This will build your website into either _ site files, or public, if you've added `destination: public` in your config.yml file, like we recommended
  * Don't forget to add public into your gitignore file
1. Open your GitHub account
2. Create new repository
3. Name your repo (often the name your website will be), select public, don't worry about a license or a README for now, and click create
4. You are going to push your local repo up to GitHub
   * Make sure HTTPS is selected
   * Copy and execute the code under *How to push an existing repository from command line* into your terminal
7. `Git push origin master` in your terminal for all pushes into GitHub
8. Get a domain name from [Namecheap.com](https://www.namecheap.com/)
9. Sign up at [Netlify.com](https://www.netlify.com/), and connect your GitHub account (sign in and authorize)
10. Attach your Namecheap domain to Netlify  
      * Go to your domain service (Namecheap), then domains > manage > add the correct nameservers for Netlify (find the nameservers Netlify requires inside the domain settings in Netlify)
      * Eventually (24-hours), your Jekyll/Netlify hosted site will connect with your domain name and it will be encrypted via HTTPS
11. Netlify will regularly grab from your GitHub repo and update your site

[Back to home]({% link index.markdown %})
