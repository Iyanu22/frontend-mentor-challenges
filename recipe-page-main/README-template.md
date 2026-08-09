# Frontend Mentor - Recipe page solution

This is a solution to the [Recipe page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/recipe-page-KiTsR8QQKm). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
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

- View the optimal layout for the recipe card depending on their device's screen size
- See hover and focus states for all interactive elements on the page

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow
- Fluid sizing with `clamp()`

### What I learned

This challenge was a good exercise in building a fully responsive card without media queries, using `clamp()` for spacing, typography, and the recipe image instead:

```css
.recipe-image{
   width: clamp(18rem, 35.5vw + 12rem, 36.5rem);
   height: clamp(10rem, 5vw + 3rem, 12rem);
   border-radius: 10px;
   object-fit: cover;
}
```

Centralizing the color palette as CSS custom properties on `:root` also made it easy to keep the rose, stone, and brown tones consistent across the preparation, ingredients, and nutrition sections:

```css
:root{
    --stone-100: hsl(30, 54%, 90%);
    --rose-800: hsl(332, 51%, 32%);
    --brown-800: hsl(14, 45%, 36%);
}
```

### Continued development

- Fix the class naming: `.Ingredients` is currently reused on the Instructions section and the Nutrition heading, which should be renamed to something more accurate like `.instructions`
- Add explicit `:hover` / `:focus` styles for the attribution links
- Swap the placeholder favicon/image paths for the actual challenge assets before deploying

### Useful resources

- [MDN - clamp()](https://developer.mozilla.org/en-US/docs/Web/CSS/clamp) - used this to build fluid sizing for the recipe image and spacing without writing separate media queries.

## Author

- Frontend Mentor - Coded by Iyanuoluwa