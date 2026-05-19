# pharbison.dev

Personal website and blog source for Patrick Harbison built with Hugo.

## Overview

This repository contains the Hugo site source for `pharbison.dev`, a platform engineering and infrastructure automation blog.

The site uses:

- Hugo static site generator
- `github.com/gurusabarish/hugo-profile` theme
- Go modules for dependency management

## Repository Structure

- `archetypes/` — default front matter for new content
- `assets/` — project assets used by Hugo pipelines
- `content/` — blog posts and page content
- `layouts/` — custom Hugo templates
- `static/` — static files deployed to the site root
- `themes/` — local theme support or theme submodule content
- `hugo.yaml` — Hugo site configuration
- `go.mod` — Go module configuration for Hugo theme and dependencies

## Prerequisites

- Go `1.25` or later
- Hugo installed (`hugo` command available)

## Local Development

Start the local Hugo server:

```bash
hugo serve
```

Then open the local server URL printed by Hugo, usually `http://localhost:1313`.

## Build

Generate the public site into the `public/` directory:

```bash
hugo
```

## Add New Content

Create new content using the existing archetype structure, or add Markdown files under `content/posts/`.

Example:

```bash
hugo new posts/my-new-post/index.md
```

## Deployment

The generated static site lives in `public/` after running `hugo`.

Deploy the contents of `public/` to your chosen hosting provider.

## Notes

- The site base URL is configured in `hugo.yaml` as `https://pharbison.dev`.
- Google Analytics is enabled via the configured tracking ID.
