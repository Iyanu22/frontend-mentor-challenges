# QR Code Component

A simple, responsive QR code component built as part of a Frontend Mentor challenge. The card displays a QR code alongside a heading and description, styled to match the provided design.

## Screenshot

![QR code component preview](./preview.jpg)

## Built With

- Semantic HTML5
- Google Fonts (Outfit)
- Mobile-first responsive design

## What I Learned

This challenge reinforced a few things I'd only half-understood before:

- **Font loading matters** — linking to a Google Fonts *browsing page* instead of the actual stylesheet endpoint silently fails with no error, so the fallback font just quietly takes over. Always use the `fonts.googleapis.com/css2?...` link, not the specimen page.
- **Percentage-based sizing has hidden gotchas** — `height: 100%` on an image doesn't behave the way `width: 100%` does unless the parent has a defined height, and vertical margins/padding in percentages are calculated relative to the parent's *width*, not height. This caused some unexpected sizing issues I had to debug.
- **Git folder structure mistakes compound quickly** — moving files around manually without checking the resulting structure led to nested duplicate folders and diverging git histories. I learned to verify folder structure with `Get-ChildItem -Recurse -Directory` before committing, and that sometimes starting a repo fresh is faster than untangling a messy git history.
- **GitHub Pages requires either a public repo or a paid plan** for private repos, and the source `index.html` must sit at the root of whichever branch/folder is selected in Pages settings.

## Author

- Iyanu(https://github.com/Iyanu22)