---
title: Quick Guide - Creating Posts in Jekyll
date: 2025-02-10
categories: [Jekyll, Tutorial]
tags: [jekyll, markdown, guide]
---

## Creating a New Post in Jekyll

### Basic Steps

Start the server with ```bundle exec jekyll s``` for a localhost.

1. Navigate to your `_posts` folder:
```bash
cd _posts
```
2. Create a new file with the following naming pattern:
```
YYYY-MM-DD-title.md
```
	For example: 2025-02-10-hellothere.md


### Extended Front Matter Options
```yml
---
# Basic Options
title: Your Post Title
date: 2024-02-10
categories: [Main Category, Sub Category]
tags: [tag1, tag2]

# Additional Options
author: your_name
pin: true    # pins post to top
math: true   # enables math formatting
mermaid: true # enables mermaid diagrams
image:
  path: /path/to/image.jpg
  alt: Image description
---
```

#### Markdown Tips
```md
## Second Level
### Third Level
#### Fourth Level
```

#### Text Formatting
```md
**Bold Text**
*Italic Text*
`inline code`
```

#### Code Blocks
```python
def hello():
    print("Hello World!")
```

#### Links and Images
```md
[Link Text](URL)
![Image Alt Text](/path/to/image.jpg)
```

#### Lists
```md
1. First item
2. Second item
   - Sub-item
   - Another sub-item
3. Third item
```


Remember to check the post in your local server before pushing to GitHub!

### Push to deploy to Github

Navigate to the ```github/workflows``` folder ```pages-deploy.yml```

Its going to run a deployment script to push it to Github pages.

```bash
git status
```
```bash
git add .
```
```bash
git status
```
This should be green, so these files are "staged".

```bash
git commit -m "feat(post):Hello There!"
```
Commiting and giving it a comment. Then push with 
```bash
git push
```
