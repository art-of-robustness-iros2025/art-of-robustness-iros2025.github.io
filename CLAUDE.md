# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Jekyll-based static website for the **IROS 2025 Workshop: "The Art of Robustness: Surviving Failures in Robotics"**. The site uses the [Minimal Mistakes](https://github.com/mmistakes/minimal-mistakes) remote theme and is hosted on GitHub Pages.

## Development Commands

### Starting the Development Server

```bash
bundle exec jekyll serve --livereload
```

This starts the local server at http://127.0.0.1:4000 with live reload enabled. The site will automatically rebuild when you make changes to files.

**Important:** Changes to `_config.yml` require a server restart to take effect.

### Ruby 3.4.1 SSL Certificate Issue

This project uses Ruby 3.4.1, which has a known SSL certificate verification bug with OpenSSL 3 on macOS (see [ruby/openssl#949](https://github.com/ruby/openssl/issues/949)). The fix is already configured in `~/.zshrc` via the `RUBYOPT` environment variable, which loads `~/.rubyopenssl_default_store.rb` automatically.

If you encounter SSL errors when downloading the remote theme, ensure your shell has the fix loaded by checking:
```bash
echo $RUBYOPT
```

It should include `-r$HOME/.rubyopenssl_default_store.rb`.

### Building for Production

```bash
bundle exec jekyll build
```

This generates the static site in the `_site/` directory.

## Site Architecture

### Key Files and Directories

- **`_config.yml`** - Main Jekyll configuration file containing:
  - Site metadata (title, description)
  - Theme configuration (`minimal_mistakes_skin: air`)
  - Plugin configuration
  - Default layouts for pages
  - Important: Changes require server restart

- **`_pages/`** - All website pages, each with YAML front matter defining:
  - `permalink` - The URL path for the page
  - `layout` - The Jekyll layout to use (typically `single` or `splash`)
  - Custom variables (e.g., speakers, organizers, sponsors arrays)

- **`_data/navigation.yml`** - Defines the main navigation menu structure

- **`assets/images/`** - All images organized by category:
  - `invited_speakers/` - Speaker profile photos
  - `organizers/` - Organizer profile photos
  - `sponsors/` - Sponsor logos
  - `gallery/` - Topic category images
  - `posters/` - Poster session photos
  - `awards/`, `talks/`, `others/` - Additional workshop media

- **`Gemfile`** - Ruby dependencies, using `github-pages` gem for GitHub Pages compatibility

### Content Structure

The site uses a **page-based structure** (not blog posts). Main pages:
- **`home.md`** - Landing page (`permalink: /`) using `splash` layout with extensive front matter data for speakers, organizers, and sponsors
- **`programme.md`** - Workshop schedule
- **`posters.md`** - Call for contributions
- **`attending.md`** - Venue and logistics information
- **`organisation.md`** - Organizer details

### Front Matter Data Pattern

The `home.md` page demonstrates the site's data pattern - complex arrays defined in YAML front matter and rendered using Liquid templates:

```yaml
invited_speakers:
  - name: "Prof. Name"
    affiliation: "University"
    image_path: /assets/images/invited_speakers/name.jpg
    topic: "Talk topic"
```

These arrays are then iterated over using `{% for speaker in page.invited_speakers %}` in the page content.

### Styling Approach

The site uses **inline `<style>` tags** within markdown files rather than separate CSS files. Custom styles are scoped to specific sections (e.g., `.speaker-list`, `.gallery`, `.organizer-list`).

## Making Content Changes

### Adding a New Speaker/Organizer/Sponsor

1. Add the image to the appropriate directory in `assets/images/`
2. Add an entry to the corresponding array in `home.md` front matter
3. The Liquid template will automatically render the new entry

### Adding a New Page

1. Create a new `.md` file in `_pages/`
2. Add YAML front matter with `permalink` and `layout`
3. Add navigation link to `_data/navigation.yml`
4. Default layout is `single` (set in `_config.yml` defaults)

### Modifying the Navigation

Edit `_data/navigation.yml` - changes are reflected immediately with live reload.

## Theme Customization

The site uses `remote_theme: mmistakes/minimal-mistakes` with the `air` skin. Theme customization is done through:
- `_config.yml` settings
- Inline styles in page markdown files
- Front matter variables that override theme defaults

Search is disabled (`search: false`) and RSS feed is hidden (`atom_feed: hide: true`).

## Deployment

The site is deployed automatically to GitHub Pages when pushing to the repository. The `github-pages` gem ensures local development matches the GitHub Pages build environment.
