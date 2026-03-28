# luismiguells.github.io

Personal website and blog for [Luis Miguel López Santamaría](https://luismiguells.github.io). Built with Jekyll and based on the [Klise](https://github.com/pietrobosi/klise) theme.

## Quick Start

### Prerequisites
- **Ruby** (v2.7+ recommended)
- **Bundler** (`gem install bundler`)

### Local Development
1. Clone the repository:
   ```bash
   git clone https://github.com/luismiguells/luismiguells.github.io.git
   cd luismiguells.github.io
   ```
2. Install dependencies:
   ```bash
   bundle install
   ```
3. Run the development server:
   ```bash
   bundle exec jekyll serve
   ```
4. Open [http://localhost:4000](http://localhost:4000) in your browser.

## Writing Content

This site uses `jekyll-compose` for easier content management:

- **New Post:** `bundle exec jekyll post "Post Title"`
- **New Draft:** `bundle exec jekyll draft "Draft Title"`
- **Publish Draft:** `bundle exec jekyll publish _drafts/draft-name.md`

## Customization

- **Styles:** Custom SCSS is located in `_sass/`.
- **Configuration:** Main site settings are in `_config.yml`.
- **Layouts:** Templates are in `_layouts/`.

## License
This project is licensed under the [MIT License](LICENSE).
