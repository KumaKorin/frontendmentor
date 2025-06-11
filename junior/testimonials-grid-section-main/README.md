# Frontend Mentor - Testimonials grid section solution

![Design preview for the Testimonials grid section coding challenge](./preview.jpg)

This is a solution to the [Testimonials grid section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 
## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size
### Links

- Live Site URL: [URL](http://kumakorin.github.io/frontendmentor/junior/testimonials-grid-section-main)
## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
### What I learned

First time to use CSS grid system, I learned a lot from it.

```CSS
@media (min-width: 1024px) {
    body {
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .card_list {
        display: grid;
        grid-template-columns: repeat(4, 1fr);
        grid-template-rows: repeat(2, 1fr);
        width: calc(100vw - 2rem);
        min-width: 1000px;
        max-width: 1200px;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
    }

    .card_list article:nth-child(1) {
        grid-column: 1 / 3;
    }

    .card_list article:nth-child(4) {
        grid-row: 2 / 2;
        grid-column: 2 / 4;
    }

    .card_list article:nth-child(5) {
        grid-column: 4;
        grid-row: 1 / span 2;
    }

    .card {
        margin: 1rem;
        padding: 2.2rem;
        max-width: 100%;
        box-shadow: 20px 20px 80px rgba(0, 0, 0, 0.2);
        z-index: 0;
    }

    .card:hover {
        box-shadow: 20px 20px 80px rgba(0, 0, 0, 0.5);
        scale: 1.02;
    }

    .card:active {
        box-shadow: 20px 20px 80px rgba(0, 0, 0, 0.6);
        scale: 0.98;
    }
}
```

### Useful resources

- [Learn CSS Grid - A 13 Minute Deep Dive](https://www.youtube.com/watch?v=EiNiSFIPIQE) - The basic concept of the CSS Grid system is explained with a bunch of usage examples.
