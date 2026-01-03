# 📘 Style Guide

*Product Preview Card Component*
## 1. Project Overview

This project uses a component-based, mobile-first CSS architecture with clear separation of concerns.
Key principles:

- BEM naming convention

- CSS custom properties (variables)

- Mobile-first responsive design

- Accessible and semantic HTML

- Scalable file structure

---

## 2. File Structure
```text
styles/
├── reset.css        /* Global reset & accessibility rules */
├── variable.css     /* Design tokens (colors, spacing, typography) */
├── button.css       /* Button component */
├── card.css         /* Product card component */
├── footer.css       /* Attribution footer */
├── responsive.css   /* Layout & media queries */
└── global.css         /* Imports all CSS files */
```

📌 Rule:
No styles should be written directly in `global.css`.
It is used only for imports.

---

## 3. CSS Methodology
Naming Convention: BEM
```html
.block
.block__element
.block__element--modifier
```

Examples:
```css
.card
.card__title
.card__pricing
.card__button
.card__button-icon
```
### Naming Rules

- Use kebab-case

- Avoid numbers like sec1, sec2

- Class names must be meaningful

- All component styles are scoped to their block

---

## 4. Design Tokens (CSS Variables)

All design values are defined in variable.css.

🎨 Colors
```css
--color-black
--color-grey
--color-cream
--color-white
--color-green-500   /* Primary */
--color-green-700   /* Hover / Active */
```

Usage rules:
```css
Primary button → --color-green-500

Hover / focus → --color-green-700

Secondary text → --color-grey

Page background → --color-cream
```

---

## Typography
```css
--txt-xlg   /* Large headings */
--txt-lg    /* Body large */
--txt-md    /* Body text */
--txt-sm    /* Labels / small text */
```

Fonts
-  Headings: Fraunces

- Body text: Montserrat

---

## Spacing System
```css
--space-zero  /* 4px */
--space-one   /* 8px */
--space-two   /* 16px */
--space-three /* 24px */
--space-four  /* 32px */
--space-five  /* 40px */
```
### Rule:
❌ Do not use raw px values
✅ Always use spacing variables

---
## 5. Button Component
Class
`.card__button`

### Characteristics

- Full width

- Flex layout (icon + text)

- Smooth hover & active states

- Accessible focus styles

### HTML Usage
```html
<button type="button" class="card__button">
  <i class="fa-brands fa-opencart card__button-icon" aria-hidden="true"></i>
  <span>Add to Cart</span>
</button>
```
### Interaction Rules

- Hover: background color + slight lift

- Active: reset transform

- Focus-visible: clear outline

- Icon animates horizontally on hover

---

## 6. Card Component
Standard HTML Structure
```html
<main class="card">
  <picture class="card__picture">
    <source media="(min-width: 768px)" srcset="image-desktop.jpg">
    <img src="image-mobile.jpg" alt="Product image">
  </picture>

  <section class="card__information">
    <section class="card__content">
      <p class="card__label">Perfume</p>
      <h1 class="card__title">Product Name</h1>
      <p class="card__text">Product description</p>
    </section>

    <section class="card__pricing">
      <span class="card__price">$149.99</span>
      <span class="card__old-price"><del>$169.99</del></span>
    </section>

    <button class="card__button">Add to Cart</button>
  </section>
</main>
```
### Rules

- .card is the main container only

- Internal layout uses Flexbox

- Border-radius values come from variables

- Content and pricing are separated semantically

---

7. Responsive Design
Strategy

-Mobile-first

-Layout changes handled in responsive.css

Breakpoint
```css
@media (min-width: 48em) { /* 768px */ }
```
### Desktop Behavior

- Card layout switches to horizontal

- Image width: 50%

- Content width: 50%

- Max width: 600px

### Rule:
All media queries must live in `responsive.css`.

---

## 8. Footer (Attribution)
Class
```css
.attribution
```

#Rules

- Not part of the card component

- Small font size

- Center-aligned text

- Only for credits and links

---
## 9. Reset & Accessibility

Defined in reset.css:

- `box-sizing: border-box`

- Button reset

- Responsive images

- `focus-visible` support

- `prefers-reduced-motion` respected

- Safe text wrapping

📌 Accessibility is mandatory, not optional.

---

## 10. General Rules

-  Use semantic HTML (main, section, footer)
-  Keep components isolated
-  Follow naming conventions strictly
-  Use variables for consistency
-  Write scalable, readable CSS
