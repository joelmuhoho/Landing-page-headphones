<!-- prettier-ignore -->
<div align="center">

# Headphones Landing Page

A responsive, multi-section headphones product landing page built with HTML and modular CSS.
</div>


## Overview

This project is a static marketing-style landing page for a headphones brand concept.
It focuses on visual presentation, section-based storytelling, and responsive behavior across desktop, tablet, and mobile breakpoints.

The page is split into dedicated content sections:

- Hero with navigation and lead capture form
- Design highlights with icon-based feature blocks
- Color collection showcase
- Blueprint/spec section
- Product cards and pricing
- Contact CTA and footer links

> [!NOTE]
> This is a frontend-only static project (no JavaScript app logic or backend).

## Features

- Clean single-page layout with clearly separated sections
- Modular CSS organization per page block
- Reusable utility classes for shadows and container widths
- Gradient-heavy visual style and product imagery
- Font Awesome icons and Google Fonts integration
- Responsive styles for laptop, tablet, and mobile widths

## Tech Stack

- HTML5
- CSS3 (modular files + media queries)
- Font Awesome (CDN)
- Google Fonts: Open Sans

## Project Structure

```text
.
├── index.html
├── css/
│   ├── reset.css
│   ├── main.css
│   ├── header.css
│   ├── top-jumbo.css
│   ├── design-by.css
│   ├── color-collection.css
│   ├── blue-print.css
│   ├── latest.css
│   └── footer.css
└── img/
    ├── logo.png
    ├── headphones.png
    ├── hp-black.png
    ├── hp-blue.png
    ├── hp-green.png
    ├── hp-mix-color.png
    ├── hp-orange.png
    ├── hp-pink.png
    └── headphones-landingpage.png
```

## Getting Started

### Prerequisites

- A modern browser (Chrome, Edge, Firefox, Safari)
- Optional: VS Code + Live Server extension for local development convenience

### Run Locally

1. Clone or download this repository.
2. Open the project folder.
3. Open `index.html` directly in your browser.

Optional (recommended during development):

- Serve with a local web server to get auto-refresh and consistent asset loading.
- In VS Code, you can use Live Server and open the served URL.

## Styling Architecture

- `css/main.css`: imports section styles and defines shared variables/utilities
- `css/reset.css`: Meyer reset + base defaults
- Section styles are split into dedicated files:
  - `header.css`
  - `top-jumbo.css`
  - `design-by.css`
  - `color-collection.css`
  - `blue-print.css`
  - `latest.css`
  - `footer.css`

### Theme Variables

Global color tokens are defined in `:root` in `css/main.css`:

- `--orange`
- `--lightblue`
- `--purple`
- `--blue`
- `--lightpurple`

Updating these values is the fastest way to retheme the page.

## Responsive Behavior

The layout uses section-level media queries with common breakpoints:

- `max-width: 1215px` (laptop adjustments)
- `max-width: 1023px` (tablet layout shifts)
- `max-width: 767px` (mobile stacking and simplification)

> [!TIP]
> If you customize spacing or image sizes, validate each section at all three breakpoints, since many components switch from side-by-side to stacked layout.

## Customization Guide

- Replace product and brand assets in `img/`
- Update headline and CTA copy in `index.html`
- Replace placeholder lorem text with product messaging
- Adjust product prices in the `#latest` section
- Update footer links and social destinations

## Notes

- Some form fields and navigation links are currently presentational (`#` links)
- Font Awesome is loaded from CDN in `index.html`
- The project currently has no build step or package manager dependency
