# Frontend Mentor - Blog preview card solution

This is a solution to the [Blog preview card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/blog-preview-card-ckPaj01IcS). 

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)

## Overview

### Screenshot
#### Desktop
![Desktop](https://github.com/user-attachments/assets/83728b7a-cdb8-4618-8a8e-a5ff616e44c3)
#### Mobile
![mobile](https://github.com/user-attachments/assets/cdee6f11-54b5-4359-93cc-e68a07117005)
### Links

- Solution URL: [Solution](https://www.frontendmentor.io/solutions/responsive-layout-for-blog-card-I6-8AWbHDr)
- Live Site URL: [Live site](https://saurabh-mishra04.github.io/Blog-Preview-Card/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

- I have used variables in scss but never tried in pure css so this was a good experience.

```css
:root{
    --yellow: #f4d04e;
    --grey-dark: #111111;
    --grey-light: #6b6b6b;
    --white: #ffffff;
}
*,::before,::after{
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}
```
- I also added a keyboard navigation which mirrors the hover effect to meet the challenge requirement of visible hover and focus states.
```
.title:hover, .title:focus-visible{
    color: var(--yellow);
    cursor: pointer;
}
.title:focus-visible{
    outline: 2px solid var(--yellow);
    outline-offset: 4px;
}
```

## Author
- Frontend Mentor - [@Saurabh](https://www.frontendmentor.io/profile/Saurabh-Mishra04)
