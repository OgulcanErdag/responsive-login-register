![Preview](preview.png)

# Responsive Login & Registration Form

Mobile-first, accessible authentication UI built with HTML, CSS, and JavaScript.  
Toggle between **Sign in** and **Create account**, with floating labels, password reveal, and a shaped image.

## Features

- Mobile-first → enhanced for desktop layouts
- Sign in / Sign up tab switch
- Floating and fixed labels
- Password show/hide
- Keyboard and screen-reader friendly (labels, focus states, ARIA)
- Works as a static site (no backend required)
- SCSS source included, compiled CSS provided

## Tech Stack

- **HTML5** for structure
- **SCSS/CSS** for styles
- **Vanilla JavaScript** for UI behavior

## Folder Structure

```
.
├── assets
│   ├── css
│   │   └── styles.css
│   ├── scss
│   │   ├── base
│   │   │   └── _base.scss
│   │   ├── components
│   │   │   └── _breakpoints.scss
│   │   ├── layout
│   │   │   └── styles.scss
│   │   ├── pages
│   │   │   └── _login.scss
│   │   └── config
│   │       └── _variables.scss
│   ├── img
│   │   ├── bg-img.jpg
│   │   ├── icon-apple.svg
│   │   ├── icon-facebook.svg
│   │   ├── icon-google.svg
│   │   └── mask-blob.svg
│   └── js
│       └── main.js
├── index.html
├── preview.png
└── README.md
```

## Getting Started

Open `index.html` in a browser.  
Or serve locally with any static server:

```bash
# Python
python -m http.server 5500
# Node
npx serve .


## Build (SCSS → CSS)

The repository already contains compiled CSS under assets/css/styles.css.
If you edit SCSS, compile with:

npm i -D sass
npx sass assets/scss:assets/css
# or watch mode
npx sass assets/scss:assets/css --watch

Accessibility

Visible focus styles

<label for> associations

Tabs set aria-selected on change

Forms are usable with keyboard only

Customization

Colors, spacing, and radii in assets/scss/config/_variables.scss

Breakpoints in assets/scss/components/_breakpoints.scss

Form component rules in assets/scss/components/_login.scss

Browser Support

Modern evergreen browsers. No IE support.

License

MIT. Use, modify, and distribute with attribution if required by your organization.
```
