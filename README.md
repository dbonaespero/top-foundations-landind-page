# The Odin Project - Landing Page

A single-page landing site built as part of [The Odin Project](https://www.theodinproject.com/) Foundations curriculum.

This is a pure HTML + CSS project with no JavaScript and no build step. The goal was to practice layout with Flexbox and match a given design reference as closely as possible.

## Live Demo

[dbonaespero.github.io/top-foundations-landing-page](https://dbonaespero.github.io/top-foundations-landing-page/)

## What's inside

The page is split into six sections:

- **Header** - logo and navigation links
- **Hero** aka first-section - main headline, subtext, CTA button, and an image placeholder
- **Info cards** aka second-section - four illustrated items with captions
- **Quote** aka third-section - a large testimonial block with attribution
- **Call to action** aka fourth-section - a colored card with a button
- **Footer** - copyright line

## Built with

- HTML5 (div-based layout - semantic elements were not part of the assignment scope at this stage)
- CSS Flexbox for layout
- No frameworks, no dependencies, no build step - just `index.html` + `styles.css`

## Things I practiced

- Flexbox: `display: flex`, `justify-content`, `align-items`, `flex: 1`, `gap`
- Vertical centering and equal-width columns
- Styling buttons, cards, and rounded borders
- Structuring a page with reusable class names
- Writing meaningful commit messages along the way
- Using Git and GitHub for version control and deployment

## Known limitations

This is a learning project, and I left a few things intentionally simple. Here's what I'm aware of and would improve next:

- **Hardcoded values in CSS.** Spacing values like `96px` for horizontal padding, `margin: 96px 144px` for the CTA card, and other magic numbers are repeated in several places instead of being centralized (CSS variables, a shared `.container` class, or utility classes). This makes the stylesheet harder to maintain - changing one value means hunting for others.
- **No responsive design.** There are no media queries, so the layout is built for desktop only and will likely break on narrow screens. Mobile support is a separate learning step.
- **No CSS variables.** Colors (`#1F2937`, `#E5E7EB`, `#3882F6`, `dodgerblue`) are hardcoded wherever they're used. A `:root` block with variables would make the theme easier to change.
- **Limited accessibility.** Links and buttons don't have `:hover` / `:focus` states, and there are no ARIA attributes. Fine for a demo, not for production.
- **`Roboto` is declared but not loaded.** The font-family stack falls back to the system sans-serif because no `@font-face` or Google Fonts link is set up yet (that's a later topic in the curriculum). As a result, `font-weight: 300` on the quote renders as regular weight on most systems.
- **Deviations from the reference design.** The quote section uses a solid `grey` background instead of the lighter tint in the original design, and buttons have slightly different padding. These were deliberate choices, not oversights.

## Run locally

Clone the repo and open `index.html` in your browser:

    git clone https://github.com/dbonaespero/top-foundations-landing-page.git
    cd top-foundations-landing-page

No dependencies, no install, no build step.

## Acknowledgements

Design brief and project spec: [The Odin Project - Landing Page](https://www.theodinproject.com/lessons/foundations-landing-page).