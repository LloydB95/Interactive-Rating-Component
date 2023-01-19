# Frontend Mentor - Interactive rating component solution

This is a solution to the [Interactive rating component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/interactive-rating-component-koxpeBUmI). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

### The challenge

Users should be able to:

- View the optimal layout for the app depending on their device's screen size
- See hover states for all interactive elements on the page
- Select and submit a number rating
- See the "Thank you" card state after submitting a rating

### Screenshots
The Screenshot below shows the initial state and the active state of clicking the numbers
![](./screenshot1.jpg)

This screenshot shows the completed state after selecting a number and clicking "**Submit**". The number that is clicked is then shown on the **"Thank You"** state.
![](./screenshot2.jpg)

### Links

- Solution URL: [https://www.frontendmentor.io/solutions/interactive-rating-component-cKW-oya7TE](https://www.frontendmentor.io/solutions/interactive-rating-component-cKW-oya7TE)
- Live Site URL: [https://lloydb95.github.io/Interactive-Rating-Component/](https://lloydb95.github.io/Interactive-Rating-Component/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
- [Tailwind.css](https://tailwindcss.com/) - CSS Framework
- [Alpine.js](https://nextjs.org/) - Javascript Framework

### What I learned

I have learned multiple things within this project, ranging from using the **Gap** class within TailwindCSS, to using Javascript functions within Alpine.js to slim down on excessive code and produce the same result. I had not delved into Javascript before this project so I have learnt the fundamentals on how certain functions work and how I could utilise them for this component. 

This code snippet below shows how I was able to set up the **Grid Column** and the **Gap** classes. This was used to show the numbers and have them evenly spaced out within the same **Div**, aiding the correct design processes.

```html
 <div class="grid grid-cols-5 gap-5 pb-8 text-sm text-center md:gap-4 text-white/50 md:text-md">
```
This snippet shows how I was able to use the **x-bind** tag to tie the Javascript functions to the **div**. The **&&** tag seen below allowed me to only show the **"Thank You"** state after a number had been chosen and the **Submit** button had been clicked. This was also achieved by the **!=** tag, which meant if nothing had been clicked and the end user would try and click on the **Submit** button, nothing would happen.

```html
<div class="relative max-w-sm px-8 py-4 overflow-hidden shadow-lg rounded-3xl bg-dark-blue/40"
x-bind:class="submit && selection != '' ? '' :'hidden'" x-cloak>
```

### Continued development

I will continue to develop my skills using frameworks like Tailwind CSS and Alpine.js as they retain all of the core functions of site building while cutting down on excess code, speeding up load times, benefitting the end user. I will learn more Javascript functions and how best to utilise them.

### Useful resources

- [Tailwind CSS - Gap](https://tailwindcss.com/docs/gap) - This resource shows the different parameters for the **Gap** class which I had used to space out the buttons in the **div**.
- [Alpine.js - Attributes](https://alpinejs.dev/) - This resource has helped me to identify the attributes present within Alpine.js and what each one does with examples of how the can be used.

## Author

- Frontend Mentor - [@LloydB95](https://www.frontendmentor.io/profile/LloydB95)

## Acknowledgments

I have had help from a colleague with vast knowledge of Javascript and it's functions.
