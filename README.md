# Review of the Results summary component challenge

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Thoughts on the project](#thoughs-on-the-project-🚀)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Challenge Solution](#challenge-solution)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

1. View the optimal layout for the interface depending on their device's screen size.
2. See hover and focus states for all interactive elements on the page
3. **Bonus**: Use the local JSON data to dynamically populate the content

### Screenshot
![Screen shot of solution](./assets/images/solution-screenshot.png)


### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

I took this challenge to practice the some of the CSS skills I have been learning
from a CSS course. I wanted to see if I could apply them.

Observe the layout of the component: It was a one dimensional horizontal layout. This could easily be modelled with flex-boxes. 

### Left side of the Component
I observed the left side of the component and noticed that its container had a purple-gradient with rounded borders. The elements within were a bunch of text elements so I thought to myself that a flex-box would be overkill to align them. I can easily center align them by simply using the text-align property, and the margin-inline property. 

### Right side of the component
The right side of the container was kind of tricky. I first thought that it had a white background and rounded right border edges, but I noticed that the white background was seamlessly connected to the purple container on the left hand side suggesting to me that the white background is not the color of the Summary Container but rather the container of the larger background that both the left container and the right container are sitting on. Therefore the Summary container on the left does not have a background color, and the rounded edges I see are the edges of the larger container that they both share.

#### Elements in the right side of the component
I closely inspected the elements on the right hand side of the component. It was a 1 dimensional layout and so i decided to use flex-box for the layout because it was combination of text buttons and a list.

##### Reaction, Memory, Verbal, and Visual
The list of elements on the right was quite challenging for me. I ended up using an `<ul><li></li></ul>` to represent them. I am not sure if that was the right element to use. Each div element has a background color, and a 1 dimensional layout that I modelled using a flex-box.

##### Reaction, Memory, Verbal, Visual and their image icon
I ran into some alignment issues with the alignment of the image icon and the text to the left of it. I had a couple of approaches in mind.
  - Using a pseudo element to append it to the start of the div but that failed because it wasn't in the background.
  - Using it as the image-icon for the bullet list and then trying to put it inside the div container but that failed too because everytime i set my div to flexbox it fell apart.
  - I wrapped both elements in a div and then set the text beside it to have a display of inline-block but the text did not sit on the same line with the icon. The vertical alignment was slightly off. I couldn't understand why.

I decided to add the image in my html and wrap both of them in a div. I set the div to flexbox and they aligned. It was the solution I thought of initially but I wanted to see if there was a solution outside of using flexboxes. Because it looked so simple to accomplish than.


### Thoughs on the project 🚀
What are the correct headers for this project ?
- Your Result -> h2
    - 76 -> (p -> strong)
    - Great -> h3
- Summary -> h2
    - Reaction -> h4
    - Memory -> h4
    - Verbal -> h4
    - Visual -> h4

Why is the bottom not aligned on the two sides ?

Where do you create CSS variables ?
- global.css
- utils.css

Need a shared top and bottom padding


### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Desktop-first workflow








------------------------------------------------------------------------

<!-- ### What I learned

Use this section to recap over some of your major learnings while working through this project. Writing these out and providing code samples of areas you want to highlight is a great way to reinforce your own knowledge.

To see how you can add code snippets, see below:

```html
<h1>Some HTML code I'm proud of</h1>
```
```css
.proud-of-this-css {
  color: papayawhip;
}
```
```js
const proudOfThisFunc = () => {
  console.log('🎉')
}
```

If you want more help with writing markdown, we'd recommend checking out [The Markdown Guide](https://www.markdownguide.org/) to learn more.

**Note: Delete this note and the content within this section and replace with your own learnings.**





### Continued development

Use this section to outline areas that you want to continue focusing on in future projects. These could be concepts you're still not completely comfortable with or techniques you found useful that you want to refine and perfect.

**Note: Delete this note and the content within this section and replace with your own plans for continued development.**

### Useful resources

- [Example resource 1](https://www.example.com) - This helped me for XYZ reason. I really liked this pattern and will use it going forward.
- [Example resource 2](https://www.example.com) - This is an amazing article which helped me finally understand XYZ. I'd recommend it to anyone still learning this concept.

**Note: Delete this note and replace the list above with resources that helped you during the challenge. These could come in handy for anyone viewing your solution or for yourself when you look back on this project in the future.**

## Author

- Website - [Add your name here](https://www.your-site.com)
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)
- Twitter - [@yourusername](https://www.twitter.com/yourusername)

**Note: Delete this note and add/remove/edit lines above based on what links you'd like to share.**

## Acknowledgments

This is where you can give a hat tip to anyone who helped you out on this project. Perhaps you worked in a team or got some inspiration from someone else's solution. This is the perfect place to give them some credit.

**Note: Delete this note and edit this section's content as necessary. If you completed this challenge by yourself, feel free to delete this section entirely.**


## Challenge Solution
This is a solution to the [Results summary component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/results-summary-component-CE_K6s0maV). Frontend Mentor challenges help you improve your coding skills by building realistic projects.  -->