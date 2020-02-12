---
layout: post
title: Automatic Publishing
date: 2020-02-11 15:45 -0700
---
# When you're ready to publish, follow the following steps.
Don't worry if your site isn't totally finished. This process sets you up for automatic updates, so your site will update as you go.

1. Open your GitHub account
2. Create new repository
3. Name your repo, select public, don't worry about a license or a README for now, and create
4. You are going to push your local repo up to GitHub
   5. Make sure HTTPS is selected
   6. Copy and execute the code under *How to push an existing repository from command line* into your terminal
7. `Git push origin master` in your terminal to ensure all future pushes
8. Get a domain name from [Namecheap.com](https://www.namecheap.com/)
9. Sign up at [Netlify.com](https://www.netlify.com/), and connect your GitHub account (sign in and authorize)
10. Attach your Namecheap domain to Netlify  
      11. Go to your domain service (Namecheap), then domains > manage > add the correct nameservers (find the nameservers Netlify requires inside the domain settings in Netlify)
      12. Eventually, your site will connect with your domain name and it will be encrypted via HTTPS
