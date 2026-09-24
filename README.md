# GAMM/SIAM Student Chapter Ulm - Website

This repository contains the source code for the official website of the [GAMM/SIAM Student Chapter Ulm](https://studentchapter-ulm.de). 

The site is built using [Jekyll](https://jekyllrb.com/) and the [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/) theme, and is hosted for free via GitHub Pages.

##  How to Add a New Activity (Blog Post)

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
```

Write your post content here using standard Markdown! You can make text bold, add links, and more.

5. Commit and push your branch to GitHub.
6. Open a Pull Request to the `main` branch. GitHub Actions will automatically test your code to ensure it builds correctly before you can merge it.

## 🛠️ Local Setup (For Developers / Maintainers)

If you want to preview the site on your own computer before publishing, you need to run the Jekyll server locally.

### Prerequisites

* Ruby (Version 3.0 or higher recommended)
* Bundler (Install via terminal: `gem install bundler`)

### Installation & Running the Server

1. Clone this repository to your local machine:
   ```bash
   git clone [https://github.com/GAMM-Student-Chapter-Ulm/GAMM-Student-Chapter-Ulm.github.io.git](https://github.com/GAMM-Student-Chapter-Ulm/GAMM-Student-Chapter-Ulm.github.io.git)
   ```
2. Navigate into the directory:
   ```bash
   cd GAMM-Student-Chapter-Ulm.github.io
   ```
3. Install the required Ruby gems (dependencies):
   ```bash
   bundle install
   ```
4. Start the local server with live-reloading:
   ```bash
   bundle exec jekyll serve --livereload
   ```
5. Open your web browser and go to `http://127.0.0.1:4000/`. The page will automatically refresh when you save changes to any file.

## 📁 Folder Structure Guide

* `_posts/`: Contains all the "Activities" (blog posts).
* `_pages/` (or root): Contains static pages like `people.md`, `contact.md`, etc.
* `_data/navigation.yml`: Controls the links in the top header menu.
* `assets/images/`: Upload all your photos and logos here. You can reference them in posts via `![Alt text](/assets/images/your-image.jpg)`.
* `_config.yml`: The main configuration file. Change site titles, footer links, and theme settings here.

## ⚖️ Handover Notes (Important!)

If you are taking over the maintenance of this site from previous students, please make sure to update the Impressum (`impressum.md`) and Datenschutzerklärung (`datenschutz.md`).

* Update the names under "Vertreten durch" to the current Chapter President / Vice President.
* Update the "Stand: [Datum]" at the top of those files to reflect when they were last checked.