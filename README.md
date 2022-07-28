# Frontend Mentor - Huddle landing page with curved sections solution

This is a solution to the [Huddle landing page with curved sections challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/huddle-landing-page-with-curved-sections-5ca5ecd01e82137ec91a50f2). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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

- View the optimal layout for the site depending on their device's screen size
- See hover states for all interactive elements on the page

### Screenshot

![](./screenshot.png)
the path for sceenshot of my solution for desktop view: screenshot-of-my-solution\huddle landing page desktop view.png
the path for sceenshot of my solution for mobile view: screenshot-of-my-solution\huddle landing page mobile view.png

### Links

- Solution URL: [solution URL ](https://your-solution-url.com)
- Live Site URL: [live site URL](https://aemrobe.github.io/huddle-with-curved-section/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

in this challenge I have learned that how can I use pseudo element to add unique shapes to your website.

to see how we can add code snippets to add unique shapes to our website.

- I want to add curved shape at the top and bottom of this div element with a class of service.

```
HTML
 <div class="service service-1">
        <div class="wrapper">
          <img
            class="service-img"
            src="./images/illustration-grow-together.svg"
            alt=""
          />
          <div class="service__wrapper">
            <h2 class="service__heading">Grow Together</h2>
            <p class="service__text">
              Generate meaningful discussions with your audience and build a
              strong, loyal community. Think of the insightful conversations you
              miss out on with a feedback form.
            </p>
          </div>
        </div>
  </div>
```

- inorder to add the curved shape at the top of this div element with a class of service. I will create the before pseudo element next I will give height to it then I will add the curved shape image as the background image inside the pseduo element finally, I will position the pseudo element outside the parent element using position absolute .

```
  CSS
  .service-1 {
  background: var(--Very-Pale-Blue);
  position: relative;
}

/*it will add the curved shape at the top of the div element*/

.service-1::before {
  content: "";
  background: url("../images/bg-section-top-mobile-1.svg");
  background-position: top left;
  background-repeat: no-repeat;
  background-size: 100% 100px;
  display: block;
  width: 100%;
  height: 100px;
  position: absolute;
  bottom: 100%;
  left: 0;
}
```

- we can use the same method to add the curved shape at the bottom of this div element the only difference is we use the after pseudo element instead.

```
CSS

/*it will add the curved shape at the bottom of the div element*/

.service-1::after {
  content: "";
  background: url("../images/bg-section-bottom-mobile-1.svg");
  background-position: top left;
  background-repeat: no-repeat;
  background-size: 100% 100px;
  display: block;
  width: 100%;
  height: 100px;
  position: absolute;
  top: 100%;
}
```

### Continued development

for the future projects I want to sharpen my skill in css grid css animation and I also want to learn javascript.

## Author

- Frontend Mentor - [@aemrobe](https://www.frontendmentor.io/profile/aemrobe)
- Twitter - [@Aemro112](https://www.twitter.com/Aemro112)

## Acknowledgments

I really want to thank @Grace from frontendmentor she has helped me how can I create the curved shape using the pseudo elements. I also want to thanks my teammates who have always helped me when I am stuck on something to work on the project.
