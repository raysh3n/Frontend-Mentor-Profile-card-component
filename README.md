# Frontend Mentor - Profile card component solution

This is a solution to the [Profile card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/profile-card-component-cfArpWshJ). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

- Build out the project to the designs provided

### Screenshot

![](./screenshot.jpg)

Add a screenshot of your solution. The easiest way to do this is to use Firefox to view your project, right-click the page and select "Take a Screenshot". You can choose either a full-height screenshot or a cropped one based on how long the page is. If it's very long, it might be best to crop it.

Alternatively, you can use a tool like [FireShot](https://getfireshot.com/) to take the screenshot. FireShot has a free option, so you don't need to purchase it.

Then crop/optimize/edit your image however you like, add it to your project, and update the file path in the image above.

**Note: Delete this note and the paragraphs above when you add your screenshot. If you prefer not to add a screenshot, feel free to remove this entire section.**

### Links

- Solution URL: [here]()
- Live Site URL: [here]()

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

positioning the profile image

```html
<div class="card__banner">
    <img src="/images/image-victor.jpg" alt="" />
</div>
```

```css
.card__banner {
    background-image: url("/images/bg-pattern-card.svg");
    /* background-repeat: no-repeat; */
    width: 100%;
    height: 10rem;
    display: flex;
    justify-content: center;
    position: relative;
}

img {
    /* outline: 1px solid black; */
    height: 8rem;
    aspect-ratio: 1/1;
    position: absolute;
    border-radius: 50%;
    top: 60%;
    border: white 5px solid;
    object-fit: cover;

    /*left:50%;
        transform:translate(-50%,-10%); */
}
```

background positioning

```css
body {
    height: 100dvh;
    display: grid;
    place-items: center;
    background-color: var(--clr-dark-cyan);
    background-image: url("/images/bg-pattern-top.svg"),
        url("/images/bg-pattern-bottom.svg");

    background-repeat: no-repeat, no-repeat;
    /* background-size: 100%; */
    background-position: bottom 50vh right 30vw, top 50vh left 30vw;
}
```
