# Frontend Mentor - Social links profile solution

This is a solution to the [Social links profile challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/social-links-profile-UG32l9m6dQ). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- See hover and focus states for all interactive elements on the page

### Screenshot

![Desktop](https://github.com/user-attachments/assets/b7e14fda-070f-4944-86be-875edf11b647)
![Mobile](https://github.com/user-attachments/assets/ccb1a364-cf24-4617-bddc-b914f3623387)

### Links

- [Solution URL](https://www.frontendmentor.io/solutions/responsive-layout-with-keyboard-navigation-jNgnrDceaS)
- [Live Site URL](https://social-links-profile-gold-kappa.vercel.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow
- Vercel

### What I learned

This was a really good project. I learned a lot of new things as I experimented a bit. 

- I learned about these new attributes: `tabindex` and `aria-disabled` which were pretty helpful for keyboard navigation control.

```html
<a href="index.html" data-status="coming-soon" tabindex="-1" aria-disabled="true">LinkedIn</a>
```

- I learned a lot of new Vanilla CSS techniques:
  - How to use a custom font from a local path instead of embedding Google Fonts links:

```css
@font-face {
  font-family: 'Inter Variable';
  src: url('assets/fonts/Inter-VariableFont_slnt,wght.ttf') format('truetype');
  font-weight: 100 900;
  font-style: oblique -10deg 0deg;
  font-display: swap;
}
```

  - Using `:not()` to exclude elements that meet certain conditions.
  - Using attribute selectors like `a[data-status="coming-soon"]` to target specific hyperlinks.

Combining them allowed me to style only the active links on focus:

```css
.links a:not([data-status="coming-soon"]):focus-visible {
    outline: 2px solid var(--green);
    outline-offset: 4px;
}
```

  - I also learned how to change the cursor behavior to indicate disabled states:

```css
.links a[data-status="coming-soon"] {
  cursor: not-allowed;
  opacity: 0.9;
}
```

### Continued development

I want to continue learning more interesting things like this and learn a bit more about Vanilla CSS properties.

### Useful resources

- [Markdown Syntax Guide](https://www.markdownguide.org/basic-syntax/) - This helped me format this file.
- [MDN HTML Docs - Tabindex](https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Global_attributes/tabindex) - This is an amazing article which helped me understand tabindex and keyboard control. I'd recommend it to anyone still learning this concept.

### AI Collaboration

- I used GitHub Copilot to understand architectural concepts and summarize documentation rather than generating the code directly. It worked well to save time digesting the docs without skipping the core coding practice.

## Author

- Frontend Mentor - [@Saurabh](https://www.frontendmentor.io/profile/Saurabh-Mishra04)
