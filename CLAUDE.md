# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

An unofficial owner's guide for KTM 500 EXC-F motorcycles, built with mdbook and deployed to GitHub Pages at
https://scode.github.io/ktm-500-exc-f/

## Commands

```bash
mdbook serve    # Local development server with hot reload
mdbook build    # Build the book to ./book/
dprint check    # Check formatting
dprint fmt      # Fix formatting
```

## Structure

- `src/` - mdbook source files (SUMMARY.md defines navigation)
- `book.toml` - mdbook configuration
- `dprint.json` - formatter config (markdown line width: 120, text wrap: always)

## CI/CD

- **CI**: Runs `dprint check` on push/PR to main
- **Deploy**: Builds and deploys to GitHub Pages on push to main
