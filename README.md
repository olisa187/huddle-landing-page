# Frontend Mentor - Huddle landing page with single introductory section solution

This is a solution to the [Huddle landing page with single introductory section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/huddle-landing-page-with-a-single-introductory-section-B_2Wvxgi0). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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
  This challenge was built for both different screen size users. 

### Screenshot

![huddle-desktop](Screenshot-desktop.png)
![huddle-mobile](Screenshot-mobile.png)

### Links

- Solution URL: [GitHub](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Desktop-first workflow

### What I learned

I learnt how to style up a link social media icons used font awesome icons. During the development stage of this huddle page I found it difficult to make the colors of both border and font change at the same time so I had to remove the link tag from the initial div that it was placed before and made the link tag itself a flex container thereby making it to have its own height, width, border.

finally when I hover over this link tag I was able to make it change its border and font color at the same time leaving out the background color.

```html
<div class="social">

    <a href="https://www.facebook.com/olisa187" class="facebook">
        <i class="fa fa-facebook" aria-hidden="true"></i>
    </a>

    <a href="https://www.twitter.com/olisa187" class="twitter">
        <i class="fa fa-twitter" aria-hidden="true"></i>
    </a>

    <a href="https://www.instagram/" class="instagram">
        <i class="fa fa-instagram" aria-hidden="true"></i>
    </a>
</div>
```
```css
.social {
    display: flex;
    justify-content: flex-end;
}

.social a {
    display: flex;
    border: 1px solid white;
    width: 2.0em;
    height: 2.0em;
    border-radius: 50%;
    color: white;
    text-decoration: none;
    align-items: center;
    justify-content: center;
}

.social a+* {
    margin-left: 1em;
}

.social a:last-child {
    margin-right: 1em;
}

.social a:hover,
.social a:active {
    border-color: hsl(300, 69%, 71%);
    color: hsl(300, 69%, 71%);
}
```

### Continued development
Still improving in my less code good output.


## Author

- Frontend Mentor - [@olisa187](https://www.frontendmentor.io/profile/olisa187)
- Twitter - [@olisa187](https://www.twitter.com/olisa187)

## Acknowledgments

Frontendmentor.io