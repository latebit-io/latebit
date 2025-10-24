# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Mentality
you love retro but you like the functionality of modern times, always have a classic 80s retro look when designing anything for this project. Also it must remain monochrome black and green terminal user interface style.

## Project Overview

This is a static website for latebit.io featuring a retro-styled landing page with an animated green grid background. The site is purely client-side HTML/CSS with no build process or dependencies.

## Repository Structure

- `index.html` - Main landing page with inline CSS styling
- `latebitflip.png` - Logo image
- `fritz-pixel.png` - Profile image
- `README.md` - Basic project description

## Development

### Running Locally

Since this is a static site with no build process, simply open the HTML file in a browser:

```bash
open index.html
```

Or use a local web server for a more realistic testing environment:

```bash
python3 -m http.server 8000
# Then navigate to http://localhost:8000
```

### Deployment

This repository is designed to be deployed as a static site. The git history shows updates to `index.html` are deployed directly.

## Code Architecture

### Styling Approach

All CSS is inline within `index.html` using a `<style>` tag. The site uses:
- Google Fonts ("Press Start 2P" for retro pixel font)
- CSS Grid background animation via keyframes
- Black background with green (#00ff00) grid lines for retro aesthetic
- z-index layering to keep content above animated background

### Animation

The grid background uses a CSS animation (`moveGrid`) that runs infinitely over 300 seconds, creating a subtle motion effect by shifting the `background-position`.

### Color Scheme

- Background: Black (#000000)
- Grid lines: Bright green (#00ff00)
- Text: White (#ffffff)
- Borders: Green (#00ff00)
