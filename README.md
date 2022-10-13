# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U).

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Links

- Solution URL: [https://github.com/leo-jcq/nft-preview-card](https://github.com/leo-jcq/nft-preview-card)
- Live Site URL: [https://leo-jcq.github.io/nft-preview-card/](https://leo-jcq.github.io/nft-preview-card/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

The main difficulty was to make the hover work on the main image to make the eye appear.

Here is my solution but I don't think it's very clean :
```html
<div id="main-image">
  <img src="./images/image-equilibrium.jpg" alt="Equilibrium">
  <div id="view">
    <div></div>
    <img src="./images/icon-view.svg" alt="">
  </div>
</div>
```
```css
#main-image {
  display: flex;
  justify-content: center;
  align-items: center;

  position: relative;

  border-radius: 7px;
}

#main-image>img {
  width: 300px;
  height: 300px;

  border-radius: 7px;

  display: block;
}

#view {
  position: absolute;

  width: 100%;
  height: 100%;

  display: flex;
  justify-content: center;
  align-items: center;

  border-radius: 7px;

  cursor: pointer;
}

#view div {
  width: 100%;
  height: 100%;

  position: absolute;

  background-color: var(--cyan);
  opacity: .5;

  border-radius: 7px;

  visibility: hidden;
}

#view img {
  position: fixed;

  opacity: 1;

  visibility: hidden;
}

#view:hover * {
    visibility: visible;
}
```

### Continued development

My goal for later is to improve the appearance of the eye for the code is cleaner.

## Author

- GitHub - [@leo-jcq](https://github.com/leo-jcq)
- Frontend Mentor - [@leo-jcq](https://www.frontendmentor.io/profile/leo-jcq)
- Twitter - [@JacquetLo2](https://twitter.com/JacquetLo2)