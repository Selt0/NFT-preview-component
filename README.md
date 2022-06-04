# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![](./images/Kapture%202022-06-04%20at%2012.42.42.gif)

### Links

- Live Site URL: [https://selt0.github.io/NFT-preview-component/](https://selt0.github.io/NFT-preview-component/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- [Bulma](https://bulma.io/) - For styles
- Mobile-first workflow

### What I learned

Setting up Bulma was very easy. However, I found myself spending a lot of time going over the docs as I'm still new to using Bulma. I probably could've finished sooner if I had just used my own CSS for everything but I'm sure once I get used to the classes, it will drastically reduce the amount of time spent on creating the project.

I designed the project using mobile-first so I was shocked to see the card take up the whole width when I expanded my browser. A quick google search I realized I could set up breakpoints just by adding the device. I was also having trouble setting up the overlay on the hover. I had forgotten how to position the overlay on top without taking up any extra space. This is where I really found the convenience of using a libray. All I had to do was add <code>is-overlay</code> and poof.

```html
<div class="columns hero-body is-variable is-0-mobile is-0-tablet mb-0">
     <div class="column is-6-tablet is-offset-3-tablet is-5-desktop is-offset-4-desktop is-4-widescreen is-offset-4-widescreen is-3-fullhd is-offset-4-fullhd">
      </div>

      <div class="is-overlay">
      </div>
</div>
```

I had a few issues with the default styling but I reminded myself I could add my own styles to override the defaults. Frameworks are meant to reduce the time to set up the project and get going. Nothing is set in stone, it's just a template.

```css
@media screen and (min-width: 1216px){
  .column.is-offset-4-widescreen {
    margin-left: 37.5%;
  }
}

```

### Continued development

I can see why having a solid foundation on HTML and CSS is vital. Although you can do mostly everything using a library, you will still need to add your own custom properties and even override those that come with the library. I'll check out other frameworks to continue expanding my tools and knowledge.

## Author

- Website - [Michael Martinez](https://michael-martinez.netlify.app/)
- Twitter - [@MMocomochi](https://www.twitter.com/MMocomochi)
