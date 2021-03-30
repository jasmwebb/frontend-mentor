# Frontend Mentor - FAQ accordion card solution

This is a solution to the [FAQ accordion card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/faq-accordion-card-XlyjD0Oam). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the component depending on their device's screen size
- See hover states for all interactive elements on the page
- Hide/Show the answer to a question when the question is clicked

### Screenshot

![](./screenshot.jpg)

## My process

### Built with

- ARIA properties
- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

#### `:target`

The `:target` CSS pseudo-class can be used to conditionally style *targeted* elements in lieu of JavaScript. In this case, I can set each FAQ answer to `display: none`, unless it is the target.

#### Accessibility

- [ ] Make the accordion an unordered list (`ul`) so a visually impaired user knows how many elements there are.
  * Give the `ul` an `aria-label` so they know it is an accordion.
- [ ] Make each question a `button` so they are tab-able by keyboard and accessible to screen readers.
  * Give each `button` an `aria-controls` attribute associated with the `id` of the content it will reveal (its answer)...
  * and an `aria-expanded` attribute whose value is `true` when the answer is toggled, otherwise `false`.
- [ ] Each answer should have...
  * an `id` that corresponds to the value of its `button`'s `aria-controls` attribute
  * an `aria-hidden` attribute whose value is `true` when the content isn't displayed, otherwise `false` (this is probably unnecessary if the `display` CSS property is toggling between `none` and `block`)

### Useful resources

- [MDN Web Docs | :target](https://developer.mozilla.org/en-US/docs/Web/CSS/:target) - Documentation for the `:target` CSS pseudo-class.
- [Carnegie Museums of Pittsburgh Web Accessibility Guidelines v1.0 | Accordions](http://web-accessibility.carnegiemuseums.org/code/accordions) - Laid out guidelines, with explanations, of how to make accordions accessible.
- [Andy Bell's Modern CSS Reset](https://piccalil.li/blog/a-modern-css-reset) - A good base for styling.

## Author

- Website - [jasminewebb.dev](https://www.jasminewebb.dev)
- Frontend Mentor - [@jasmwebb](https://www.frontendmentor.io/profile/jasmwebb)
