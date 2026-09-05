# 4ORM — Sign-Up Form

A stylized sign-up page built as a practice project for **[The Odin Project](https://www.theodinproject.com/lessons/node-path-intermediate-html-and-css-sign-up-form)** curriculum. The goal of this exercise was to design and build a polished, responsive-minded sign-up form using semantic HTML and hand-written CSS — no frameworks, no libraries.

**Live Demo:** [4ORM](https://carnocentaurus.github.io/sign-up-form/)

> ⚠️ **Disclaimer:** 4ORM is **not a real product or service**. This project is **frontend only** — there is no backend, no database, and no actual account creation. Submitting the form does not send data anywhere or create a real account. It exists purely to demonstrate HTML/CSS layout, styling, and form-building skills as part of The Odin Project's coursework.

## Overview

The page is split into two halves:

- **Left panel** — a full-height background image with a logo overlay, meant to set the visual tone of the (fictional) brand.
- **Right panel** — a three-part content area containing:
  1. Introductory marketing copy
  2. The sign-up form itself (first/last name, email, phone number, password, confirm password)
  3. A call-to-action button with a "log in" prompt

## Features

- Custom `@font-face` declarations for two fonts (`Brunson` for headings/labels, `Roboto` for body text), each with `woff2` → `woff` → `ttf` fallbacks and `font-display: swap` for better perceived load performance.
- Font preloading via `<link rel="preload">` for the primary `.woff2` files.
- Native HTML form validation using `minlength`, `type`, and `pattern` attributes (e.g. email, tel, password fields), with custom `:user-invalid` styling to visually flag invalid input.
- Custom-styled inputs, placeholders, and focus states (no default browser outlines).
- Two-column layout for form fields using simple `<ul>` groupings.
- Hover states on the submit button for interactivity feedback.
- Clean CSS reset (`* { margin: 0; padding: 0; box-sizing: border-box; }`) as a baseline.

## Built With

- **HTML5** — semantic structure, native form validation attributes
- **CSS3** — Flexbox layout, custom fonts, pseudo-classes/elements (`:focus`, `:user-invalid`, `::placeholder`)
- No JavaScript, frameworks, or build tools are used in this version

## Project Structure

```
.
├── index.html
├── style.css
├── fonts/
│   ├── Brunson.woff2 / .woff / .ttf
│   └── Roboto-Regular.woff2 / .woff / Roboto.ttf
├── images/
│   ├── form-svgrepo-com.svg
│   └── milad-fakurian-_zSZVxZWhkY-unsplash.jpg
└── README.md
```

## Getting Started

Since this is a static frontend project with no dependencies, you can run it locally with just a browser:

1. Clone or download this repository.
2. Make sure the `fonts/` and `images/` folders (with the assets referenced in `style.css` and `index.html`) are present alongside `index.html`.
3. Open `index.html` directly in your browser, or serve it with a simple local server (e.g. the VS Code "Live Server" extension) for the best results with font preloading.

No installation, build step, or package manager is required.

## What This Project Does *Not* Do

To be explicit, since this is a learning exercise:

- ❌ No backend or server — the `<form>` `action` is empty and submission is not wired up to anything
- ❌ No real account creation, authentication, or data storage
- ❌ No JavaScript-based form handling or validation beyond native HTML attributes
- ❌ No "Log in" functionality — it's a static label only

## Credits

- - Photo by [Milad Fakurian](https://unsplash.com/@fakurian?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText) on [Unsplash](https://unsplash.com/photos/a-black-and-white-photo-of-a-curved-object-_zSZVxZWhkY?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)
- Form icon from [SVG Repo](https://www.svgrepo.com/svg/457957/form)
- Project brief and guidance from [The Odin Project](https://www.theodinproject.com/) curriculum

## License

This project was built for educational purposes as part of The Odin Project coursework and is free to reference or reuse for learning purposes.