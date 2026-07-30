# Blog Preview Card

A responsive blog preview card built as a Frontend Mentor challenge. The card displays an article illustration, category tag, publish date, title, description, and author — matching the provided design at both mobile and desktop breakpoints.

## Screenshot

![Blog preview card](./preview.jpg)

<!-- Update the path above to match your actual screenshot filename/location -->

## Links

- Live Site: [Add your GitHub Pages URL here]
- Repo: [Add your repo link here]

## Built With

- Semantic HTML5
- CSS3 (Flexbox, mobile-first media queries)
- Self-hosted web font (`@font-face` with Outfit)
- Mobile-first responsive design (375px – 1440px)

## What I Learned

- **Mobile-first is the more forgiving approach** — writing base styles for the smallest screen first, then adding `min-width` media queries for larger breakpoints, avoided a lot of the overflow and cramped-spacing issues I hit when I tried sizing things with a fixed percentage width instead.
- **`box-sizing: border-box`** is worth setting globally early on — without it, padding was pushing my card wider than the viewport on smaller screens.
- **Compare designs at both breakpoints before assuming anything changes** — in this challenge the card itself stayed the same size on mobile and desktop; only the surrounding space changed. Checking both screenshots side by side saved me from writing an unnecessary media query that would've made the desktop card too wide.
- **Double-check the HTML actually includes every visual element from the design** — I initially left out the article illustration image entirely and didn't catch it until comparing my rendered output directly against the reference screenshots.

## Author

- Iyanu (https://github.com/Iyanu22)