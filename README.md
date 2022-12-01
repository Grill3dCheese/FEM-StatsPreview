# Frontend Mentor - Stats preview card component solution

This is a solution to the [Stats preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size

### Screenshot

Mobile Screenshot:
![](design/mobileScreenshot.png)

Desktop Screenshot:
![](design/desktopScreenshot.png)

### Links

- Solution URL: [https://github.com/Grill3dCheese/FEM-StatsPreview](https://github.com/Grill3dCheese/FEM-StatsPreview)
- Live Site URL: [https://grill3dcheese.github.io/FEM-StatsPreview/](https://grill3dcheese.github.io/FEM-StatsPreview/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties & animation
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

This project helped me:

- Use the HTML picture element again to understand how to best implement multiple images at different viewport sizes
- Learn to use the :root CSS selector to create variables!
- Realize the @import statement needs to come before any/all other stylings
- Also found that when I ran the lighthouse audit on the project while utilizing the CSS @import for the Google fonts it came back with a performacne rating of 96. However, when using the link element in the HTML file, lighthouse reported performance at 99! Going forward I'll continue to include fonts via the link element in the HTML file.
- Continue to better understand CSS grid and Flexbox - was able to include the picture element early on in the HTML code which put the image on top when in mobile. Then, using CSS grid, I was able to specify "order" attribute to get the picture to come second/after the content on the desktop version. Also, sometimes Flex is better utilized over grid and vice versa - it seems like grid is best for layouts whereas flex is good for positioning and alignment.

```html
<link rel="preconnect" href="https://fonts.googleapis.com" />
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
<link
  href="https://fonts.googleapis.com/css2?family=Inter:wght@400;700&family=Lexend+Deca&display=swap"
  rel="stylesheet"
/>
```

```css
:root {
  --clr-primary-800: hsl(233, 47%, 7%);
  --clr-primary-600: hsl(244, 38%, 16%);
  --clr-secondary-100: hsl(277, 64%, 61%);

  --clr-neutral-300: hsla(0, 0%, 100%, 0.6);
  --clr-neutral-200: hsla(0, 0%, 100%, 0.75);
  --clr-neutral-100: hsl(0, 0%, 100%);

  --ff-base: "Inter", sans-serif;
  --ff-accent: "Lexend Deca", sans-serif;

  --fw-regular: 400;
  --fw-bold: 700;
}

@keyframes scale {
  0% {
    transform: scale(1);
  }

  25% {
    transform: scale(0.9);
  }

  50% {
    transform: scale(1.1);
  }

  100% {
    transform: scale(1);
  }
}

@keyframes pulsePurple {
  0% {
    color: var(--clr-neutral-100);
  }

  50% {
    color: var(--clr-secondary-100);
  }

  100% {
    color: var(--clr-neutral-100);
  }
}
```

### Continued development

- Continue using CSS Grid and Flexbox to further knowledge of how each work and best use scenarios.
- Continue to think in a mobile-first mindset, while also implementing best accessability practices.
- CSS animations are fun!! Learn more about them!

## Author

- Website - [Keith McKenna](https://www.keithmckenna.com)
- Frontend Mentor - [@Grill3dCheese](https://www.frontendmentor.io/profile/grill3dcheese)
- Twitter - [@keithmckenna](https://www.twitter.com/keithmckenna)

## Acknowledgments

Thank you, Kevin Powell, for helping me structure my HTML and CSS files!
