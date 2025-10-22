# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Hugo static site generator project. Hugo is a fast and modern static site generator written in Go.

## Build and Development Commands

### Development Server
```bash
hugo server
```
Starts the Hugo development server with live reload. By default runs on http://localhost:1313

```bash
hugo server -D
```
Start server and include content marked as drafts

### Building the Site
```bash
hugo
```
Builds the static site into the `public/` directory

```bash
hugo -D
```
Build including draft content

### Content Management
```bash
hugo new content/posts/my-post.md
```
Create new content using the archetype template from `archetypes/default.md`

## Project Structure

- `archetypes/` - Content templates for new pages/posts
- `assets/` - Files processed by Hugo Pipes (SCSS, JS, images)
- `content/` - Markdown content files that become site pages
- `data/` - Configuration files for data-driven content
- `i18n/` - Translation files for multilingual support
- `layouts/` - HTML templates that define site structure
- `static/` - Static files copied directly to output (images, CSS, JS)
- `themes/` - Hugo themes
- `hugo.toml` - Main configuration file
- `public/` - Generated static site (created after build, not in version control)

## Configuration

The site is configured via `hugo.toml`. Key settings include:
- `baseURL` - The root URL of the site
- `languageCode` - Site language
- `title` - Site title

## Hugo Version

This project uses Hugo v0.151.2+extended (installed via Homebrew on macOS).
