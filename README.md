# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Frontend Mentor - QR code component solution](#frontend-mentor---qr-code-component-solution)
  - [Table of contents](#table-of-contents)
  - [Overview](#overview)
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

### Links

- Solution URL: [Add solution URL here](https://rmwatcher.github.io/qr-code-component-main/)
- Live Site URL: [QR-Code site](https://rmwatcher.github.io/qr-code-component-main/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

Using Flexbox to keep the contents and alignment centered while using CSS Grid to center the card itself in the middle of the screen. If it looks good mobile, it'll look just as good on desktop. That's the idea of the mobile-first approach, even if you have to make adjustments for the desktop.

There's a formula for border-radius to make them look smooth and consistent when you have two or more containers (in this case, our card where the qr code is at). The container outside the main content is the other radius while the content itself is considered the inner radius.

For this example, the image of the qr code is the inner radius while the content inside the main element is the other radius.

Here is the code below:


```css
main {
  border-radius: 20px;
}

figure img {
    border-radius: 10px;
}
```

As you can see, I made the radius of the image at 10px and the distance from the image to the edge of the main element is 10px which brought me to 20px for the radius of the main element.

**Note: I use Flexbox to center the content itself.**

One way to center your content on a webpage is using CSS Grid. That alone will center the card horizontally; however, as I discovered it didn't centered the card vertically. What you have to do is to ensure the parent container, which contains the element that teh card is in, has a defined height. Of course, hard coding a fixed height isn't ideal, but thanks to a resource from stack overflow (see below), you can input the following on your parent container which in my case will be the body element.

```css
body {
  height: 100vh;
}
```
The vh is viewport height where viewport is the browser window size and vh means relative to 1% of the height of the viewport [See W3schools](https://www.w3schools.com/cssref/css_units.php).

### Continued development

Regardless of our skill level, it's important to remember and work on the fundamentals; weather it's web dev, software, machine learning, or other areas.

This experience reminded that no matter what new skills you pick up, if you work hard on learning or relearning your fundamentals, it'll get easier to learn more advance skills that's help in your profession.

### Useful resources

- [Medium](https://medium.com/design-bootcamp/getting-your-border-radius-right-a-simple-trick-for-smooth-nested-containers-f6e0025e8c53) - This article helped me get the border radius for the main card and the image itself. Even if you're not subscribed to Medium, the image alone will give you the formula that'll make your corners look smooth and consistent.
- [Stack Overflow](https://stackoverflow.com/questions/76985911/trying-to-center-a-card-on-a-page) - This stack overflow page talks about how to center your content not just horizontally but vertically as well. Despite being over two years old and talking about this same challenge, this still holds up today.

## Author

- Website - [Richard Mora](https://richardmora.net)
- Frontend Mentor - [@RMwatcher](https://www.frontendmentor.io/profile/RMwatcher)
- GitHub - [RMwatcher](https://github.com/RMwatcher)


## Acknowledgments

I would like to give a special shout out to the people from the stack overflow page from above for providing an answer to a question I had while doing this challenge.
