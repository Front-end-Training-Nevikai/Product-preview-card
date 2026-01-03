# Frontend Mentor - Product Preview Card Component Solution

This repository contains my solution to the
[Product Preview Card Component challenge](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa) on Frontend Mentor.

Frontend Mentor challenges help developers improve their front-end skills by building realistic UI components using real-world workflows.

---

## 📑 Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [Project structure](#project-structure)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)

---

## 🔍 Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device’s screen size
- See hover and focus states for interactive elements
- Experience a responsive and accessible product card component

---

### Screenshot

![Product preview card screenshot](./assets/images/Screenshot%202026-01-02%20232205.png)

---

### Links

- **Solution URL:** [Frontend Mentor Solution](https://www.frontendmentor.io/solutions/product-preview-card-QMtWQ2A5qG)
- **Live Site URL:** [Live Demo](https://front-end-training-nevikai.github.io/Product-preview-card/)

---

## 🛠 My process

### Built with

- Semantic HTML5
- CSS Custom Properties (Variables)
- Flexbox
- Mobile-first workflow
- Responsive images using `<picture>`
- CSS `clamp()` for fluid typography and spacing
- Accessibility best practices

---

### Project structure

```text
├── assets
│   ├── images
│   │   ├── favicon-32x32.png
│   │   ├── image-product-mobile.jpg
│   │   ├── image-product-desktop.jpg
│   │   ├── screenshot.png
│   │   └── cart-icon.svg
│   └── styles
│       styles/
│       ├── reset.css
│       ├── variable.css
│       ├── button.css
│       ├── card.css
│       ├── footer.css
│       ├── responsive.css
│       └── global.css
├── index.html
├── README.md
└── .gitignore
```

---

### What I learned

In this project, I focused on improving my CSS architecture and responsive design workflow.

Key takeaways:

- Using CSS custom properties to create a reusable design system

- Writing mobile-first CSS and scaling layouts with media queries

- Applying clamp() for fluid typography instead of fixed breakpoints

- Structuring CSS files for better maintainability

- Enhancing user experience with subtle button animations and hover states

Example:
```css
.card__button {
  transition: background-color 200ms ease,
              transform 200ms ease,
              box-shadow 200ms ease;
}
```

---

### Continued development

In future projects, I want to continue improving:

- Component-based CSS architecture

- Advanced accessibility techniques

- Micro-interactions and motion design

- Refactoring projects into modern frameworks such as React

---

### Useful resources


- Great platform for realistic front-end challenges [Frontend Mentor](https://www.frontendmentor.io/)


- Reliable reference for HTML & CSS [MDN Web Docs](https://developer.mozilla.org/en-US/)


- Helpful articles on layout and modern CSS techniques [CSS-Tricks](https://css-tricks.com/)

---

## 👤 Author

Frontend Mentor – [Ali Nevikai](https://www.frontendmentor.io/profile/nevikai)
