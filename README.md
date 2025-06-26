# Frontend Mentor - Social proof section solution

This is a solution to the [Social proof section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/social-proof-section-6e0qTv_bA). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the section depending on their device's screen size

### Screenshot

![](.![alt text](image.png))

### Links

- Solution URL: (https://github.com/korcakSEA/social-proof-section-master.git)
- Live Site URL: (https://korcaksea.github.io/social-proof-section-master/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow


### What I learned

My major learnings while working through this project is deeper understanding of background images and applying different rules to place rating and testimonial parts. 

max-width, height, and border are written as rule in order to understand this placement.

You can find the code snippets, see below:


```css
.background__test{
    max-width: 375px;
    height:1530px;
    border: 1px solid red;

    background-image: url('/images/bg-pattern-top-mobile.svg'), 
                      url('/images/bg-pattern-bottom-mobile.svg');
    background-repeat: no-repeat, no-repeat;
    background-position: top left, bottom right;
}

@media (min-width:800px) {
    .background__test {
        max-width: 1400px;
        height: 800px;
        border: 1px solid blue;

        background-image: url('/images/bg-pattern-top-desktop.svg'), 
                          url('/images/bg-pattern-bottom-desktop.svg');
        background-repeat: no-repeat, no-repeat;
        background-position: top left, bottom right;
    }
}
```
```css
    .rating > div:nth-child(2){
         align-self: center;
    }

    .rating > div:nth-child(3){
        align-self:flex-end;
    }

    .testimonial{
        margin-block: 1.5rem;
    }

    .testimonial__cards{
        width: 100%;
        transform: translateY(0);
        transition: transform 0.3s ease-in-out;
    }
       
    .testimonial__cards:nth-child(2) {
        transform: translateY(1.25rem);
    }
    .testimonial__cards:nth-child(3) {
        transform: translateY(2.5rem);
    }
```
## Author

- Frontend Mentor - [@korcakSEA](https://www.frontendmentor.io/profile/korcakSEA)
