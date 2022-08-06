# Frontend Mentor - NFT preview card component

This is a solution to the [Single price grid Component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/single-price-grid-component-5ce41129d0ff452fec5abbbc). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

- Build out the project to the designs provided

### Screenshot

# Mobile Preview 

![screenshot]()

# Desktop Preview 

![screenshot]()


### Links

 - Source code: [https://github.com/romila2003/NFT-Preview-Card-Component]https://github.com/romila2003/NFT-Preview-Card-Component)
 - Live website: []()

## My process

### Built with

- Semantic HTML5 markup
- Plain CSS
- Flexbox
- Mobile-first workflow

### What I learned

This challenge was fairly simple however the hover effect was quite a challenge and struggled with that aspect of the card for a while so I read other people's code to gain a better understanding of their approach which really helped a lot. I learned new concepts to implement such as the `::before` and `::after` property.

Css Grid - code: 

```css

.img-holder::before, .img-holder::after {
    content: "";
    position: absolute;
    border-radius: 10px;
}

.img-holder::before {
    inset: 0;
    opacity: 0;
    background-color: var(--cyan);
    width: 100%;
    height: 98%;
}

.img-holder::after {
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 100%;
    aspect-ratio: 1;
    background-image: url('/images/icon-view.svg');
    background-repeat: no-repeat;
    background-position: center;
    color: var(--white);
    opacity: 0;
}

.img-holder:hover::before {
    opacity: 0.5;
}

.img-holder:hover::after {
    opacity: 1;
}
```

### Continued development

For future developments, I should use more css grids into future projects and begin taking on more challenging responsive projects to test my skills. Also, I should begin learning the basics of javascript and implementing my knowledge into the challenges. 


## Author

- Frontend Mentor - [@romila2003](https://www.frontendmentor.io/profile/romila2003)
- Twitter - [@romila003](https://www.twitter.com/romila003)

## Acknowledgments

I was inspired by [@dostonnabotov](https://www.frontendmentor.io/profile/dostonnabotov) to help me with the hover effect of the card. I learned more about pseudos and and a new concept of `aspect-ratio`.
