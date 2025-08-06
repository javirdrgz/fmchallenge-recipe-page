# Frontend Mentor - Recipe page solution

This is a solution to the [Recipe page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/recipe-page-KiTsR8QQKm). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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

## Overview

### Screenshot

![](Screenshot%20Frontend%20Mentor%20Recipe%20Page.png)

### Links

- Solution URL: [Add solution URL here](https://github.com/javirdrgz/fmchallenge-recipe-page)
- Live Site URL: [Add live site URL here](https://javirdrgz.github.io/fmchallenge-recipe-page/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

This solution is part of my practice to become more familiar with the layout principles laid down by Heydon Pickering and Andy Bell in their book "Every layout". In this simple recipe page the only layout element used was the basic "stack" and "recursive stack" where you stack elements using flexbox and tweaking the spacing.

Something I'm not convinced of is the solution I implemented to make the image full width in the mobile version. I wanted the image to be part of the article header element, but since the article had padding, that would apply to the image too. Therefore I added some CSS for the image to ignore the padding of it's parent element. I feel there has to be a better solution, so I'll be looking for it.

```css
img {
  /* ignore parent padding */
  width: calc(100% + calc(2 * var(--s1)));
  margin-left: calc(-1 * var(--s1));
  margin-top: calc(-1 * var(--s1));
  max-width: none;
}
```

### Continued development

My objective is to make the layout principles in "Every Layout" second nature. I'm looking for the ability to see a website and see how it is composed in terms of these basic layout elements.

### Useful resources

- [Every Layout](https://every-layout.dev/) - This helped me with the layout of the website. I really liked this pattern and will use it going forward.
- [Ignore parent element padding](https://stackoverflow.com/questions/4296530/ignore-parent-padding) - Stack Overflow solution.
- [MDN](https://developer.mozilla.org) - used for reference.

## Author

- Frontend Mentor - [@javirdrgz](https://www.frontendmentor.io/profile/javirdrgz)

## Acknowledgments

Thanks to Frontend Mentor for providing this challenges, to the authors of "Every Layout", to the maintainers of MDN and the people who contribute to Stack Overflow.
