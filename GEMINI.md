# Gemini Instructions: luismiguells.github.io

This project is a personal Jekyll-based static website/blog using a customized version of the [Klise theme](https://github.com/pietrobosi/klise).

## Project Overview

- **Site Title:** luismiguells
- **Owner:** Luis Miguel López Santamaría
- **Core Technology:** Jekyll 4.1.0 (Ruby), Sass, kramdown.
- **Plugins:** `jekyll-feed`, `jekyll-sitemap`, `jekyll-compose`, `jekyll-postfiles`.

## Architectural Overview

- **Framework:** Static Site Generation (SSG).
- **Styles:** Custom Sass located in `_sass/` (specifically `_sass/klise/` and `_sass/scss/`).
- **Layouts:** Standard Jekyll layouts in `_layouts/` (`default`, `home`, `post`, `page`).
- **Content:** Blog posts are organized in the `_posts/` directory. Due to `jekyll-postfiles`, each post can have its own subdirectory (e.g., `_posts/post-slug/`) containing the markdown file and local assets.

## Core Workflows

### 1. Local Development
To run the site locally for testing:
```bash
bundle install
bundle exec jekyll serve
```
The site will be available at `http://localhost:4000`.

### 2. Creating New Content
Utilize `jekyll-compose` for consistency:

- **Create a Post:**
  ```bash
  bundle exec jekyll post "Your Post Title"
  ```
- **Create a Draft:**
  ```bash
  bundle exec jekyll draft "Your Draft Title"
  ```
- **Publish a Draft:**
  ```bash
  bundle exec jekyll publish _drafts/your-draft-title.md
  ```

### 3. Image Assets
- Store images for posts in: `assets/img/posts/<post-slug>/`
- General assets: `assets/img/` or `assets/files/` (e.g., CV.pdf).

## Conventions

- **Post Front Matter:**
  ```yaml
  ---
  title: "Title of the Post"
  date: YYYY-MM-DD HH:MM:SS +TZ
  modified: YYYY-MM-DD HH:MM:SS +TZ
  tags: [tag1, tag2]
  description: "A brief summary of the post."
  ---
  ```
- **Naming:** Follow the Jekyll default `YYYY-MM-DD-title.md` for posts.

## Technical Constraints

- **Jekyll Version:** 4.1.0.
- **Theme Customization:** Most visual changes should be made within `_sass/klise/` or by overriding `_layouts/`.
- **Environment:** Requires Ruby (compatible with Jekyll 4.1) and Bundler.
