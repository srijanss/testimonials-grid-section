# Frontend Mentor - Testimonials grid section solution

This is a solution to the [Testimonials grid section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

### Screenshot

![](./images/desktop-screenshot.jpg)
![](./images/mobile-screenshot.jpg)

### Links

- Solution URL: [https://github.com/srijanss/testimonials-grid-section](https://github.com/srijanss/testimonials-grid-section)
- Live Site URL: [https://srijanss.github.io/testimonials-grid-section/](https://srijanss.github.io/testimonials-grid-section/)

## My process

```html
<figure class="testimonial__author">
  <img
    src="./images/image-daniel.jpg"
    alt="Daniel Clifford"
    class="testimonial__author-image"
    width="28"
    height="28"
  />
  <figcaption class="testimonial__author-info">
    <h3 class="testimonial__author-name">Daniel Clifford</h3>
    <p class="testimonial__author-verified">Verified Graduate</p>
  </figcaption>
</figure>
```

I learned about the html element <figure> and <figcaption> elements for semantically representing image and its caption.

```css
& .testimonial:nth-child(1) {
    position: relative;
    & > * {
      position: relative;
      z-index: 1;
    }
    .pattern-quotation {
      position: absolute;
      top: 0;
      right: 24px;
      z-index: 0;
      @mixin media-query-desktop {
        right: 80px;
      }
    }
```

I had some issues to put the quotation mark svg image behind the text. I found out that to make the z-index work we have to set CSS position propery in that element.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
- [Vite](https://vitejs.dev/) - Lightweight frontend tooling
- [PostCSS](https://postcss.org/) - Tool to transform CSS using plugins

### What I learned

## Author

- Website - [Srijan Manandhar](https://github.com/srijanss)
- Frontend Mentor - [@srijanss](https://www.frontendmentor.io/profile/srijanss)
