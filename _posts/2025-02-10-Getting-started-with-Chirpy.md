---
# Basic Options
title: Getting started with Chirpy
date: 2025-02-10
categories: [Jekyll, Tutorial]
tags: [Chirpy, Tutorial, Theme]

# Additional Options
author: "IronDingo"
pin: false    # pins post to top
math: true   # enables math formatting
mermaid: true # enables mermaid diagrams
image:
  path: https://chirpy-img.netlify.app/commons/avatar.jpg
  alt: Chirpy Jekyll Theme
---

[Getting Started with Chirpy](https://chirpy.cotes.page/posts/getting-started/)

Go to their page
"use template"
Make a good name like 
```
Mysite.github.io
```

Then 
```bash
git clone https://github.com/cotes2020/chirpy-starter.git mysite.github.io
```

Then just
```bash
bundle
```

If permission error occurs:
```bash
sudo chown eko:eko /home/eko/irondingosite/irondingo.github.io/ -R
```
Or
```bash
sudo chown $USER:$USER /home/eko/irondingosite/irondingo.github.io/Gemfile.lock
```

Then run the site locally with:
```bash
bundle exec jekyll s
```


Do the edits in _config.yml and in _posts.

Then push

Navigate to the ```github/workflows``` folder ```pages-deploy.yml```

Its going to run a deployment script to push it to Github pages.

If its there, if not continue below.

```bash
git status
git add .
git status
```
This should be green, so these files are "staged".

```bash
git commit -m "feat(post):New changes uploaded!"
```
Commiting and giving it a comment. Then push with
```bash
git push
```



{% include embed/youtube.html id='F8iOU1ci19Q' %}
