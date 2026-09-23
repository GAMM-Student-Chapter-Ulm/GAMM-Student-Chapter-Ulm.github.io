
# GAMM/SIAM Student Chapter Ulm - Website

This repository contains the source code for the official website of the [GAMM/SIAM Student Chapter Ulm](https://studentchapter-ulm.de).

The site is built using [Jekyll](https://jekyllrb.com/) and the [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/) theme, and is hosted for free via GitHub Pages.

## How to Add a New Activity (Blog Post)

Adding a new post is easy and doesn't require any coding knowledge. You just need to write a Markdown file!

1. Create a new branch: `git checkout -b your-branch-name`
2. Go to the `_posts` folder.
3. Create a new file. **The filename must follow this exact format:** `YYYY-MM-DD-title-of-post.md` (e.g., `2024-05-23-gamm-annual-meeting.md`).
4. Add the following "Front Matter" to the very top of your file, then write your content below it:

```yaml
---
title: "Your Post Title Here"
categories:
  - Activities
---

Write your post content here using standard Markdown! You can make text **bold**, add [links](https://example.com), and more.
```
