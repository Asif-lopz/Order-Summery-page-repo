# Frontend Mentor - Order summary card solution

This is a solution to the [Order summary card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/order-summary-component-QlPmajDUj). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

- See hover states for interactive elements

### Screenshot

![](solution/Order-summary-card-Desktop-View-1440px.png)
![](solution/Order-summary-card-Mobile-view-370px.png)

### Links

- Live Site URL: [CodePen](https://codepen.io/asiflopz/project/editor/AbLnqY)

## My process
I first downloaded challage website and exracted in my computer and opened Vsiual studio code and edited some html code and deleted few files
come from challager,


### Built with

- Semantic HTML5 markup
- CSS custom properties
- Mobile-first workflow

### What I learned

I learned css style position and aligment and it was my first solo coding without looking solution in Internet, Waiting for next challages
need to improve my code also

To see how you can add code snippets, see below:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <link rel="icon" type="image/png" sizes="32x32" href="./images/favicon-32x32.png">
  <link rel="stylesheet" href="intex.css">
  <title>Order summary card</title>
</head>
<body>
  <div class="container">
    <img src="images/illustration-hero.svg" alt="hero">
    <h1>Order Summary</h1>

    <p>You can now listen to millions of songs, audiobooks, and podcasts on any device anywhere you like!</p>
        
      <div class="selector">
        <img src="images/icon-music.svg" alt="music">
        <h3>Annual Plan</h3>
        <p class="price">$59.99/year</p>

        <a href="">Change</a> 
      </div>
    
    <div class="proceed"><button>Proceed to Payment</button>  </div>
    <div class="cancel"><button>Cancel Order</button> </div>
  </div>

  
  <div class="attribution">
    Challenge by <a href="https://www.frontendmentor.io?ref=challenge" target="_blank">Frontend Mentor</a>. 
    Coded by <a href="https://github.com/Asif-lopz">Asif KK</a>.
  </div>
</body>
</html>
```
```css
@import url("https://fonts.google.com/specimen/Red+Hat+Display");

body {
  width: 1440px;
  height: auto;
  margin: 0;
  padding: 0;
  background-color: hsl(225, 100%, 94%);
  text-align: center;
  font-family: "Red Hat Display";
  background-image: url("images/pattern-background-desktop.svg");
  background-repeat: no-repeat;
}
.container {
  margin: 0;
  padding: 0;
  width: 450px;
  height: auto;
  transform: translate(110%, 10%);

  background: #ffffff;
  border-radius: 20px;
}
.container img {
  border-top-right-radius: 20px;
  border-top-left-radius: 20px;
}
.container h1 {
  margin: 25px 0 25px 0;
  font-weight: 900;
  text-shadow: 0px 0px 4px rgba(0, 0, 0, 0.50);

}
.container p {
  width: 280px;
  font-size: 18px;
  height: auto;
  margin: 0 0 20px 80px;
  text-shadow: 0px 0px 2px hsl(224, 23%, 55%);
}
.selector {
  width: 300px;
  height: 70px;
  background-color: hsl(225, 100%, 98%);
  margin: 0 0 0 80px;
  border-radius: 10px;
}
.selector * {
  display: inline;
}
.selector img {
  position: relative;
  top: 15px;
  right: 80px;
}
.selector h3 { 
  position: relative;
  font-size: 15px;
  right: 60px;
  bottom: 18px;
  font-weight: 900;
  padding-bottom: 5px;
  text-shadow: 0px 0px 3px rgba(0, 0, 0, 0.50);
  
}

.selector .price, h3 {
  position: relative;
  right: 50px;
  bottom: 15px;
}
.selector .price {
  margin-bottom:1px;
}

.selector a {
  float: right;
  position: relative;
  bottom: 30px;
  right: 15px;
}

.proceed {
  margin: 30px 0 10px 0;
}
.proceed button {
  padding: 10px 100px 10px 100px;
  border-radius: 10px;
  background-color: hsl(245, 75%, 52%);
  color: white;
  box-shadow: 5px 4px 18px 2px rgba(153, 131, 250, 0.5), 0 6px 20px 0 rgba(64, 64, 65, 0.19);
  font-weight: 500;
  font-size: 13px;
}
.proceed button:hover {
  cursor: pointer;
  background-color: hsl(245, 88%, 50%);;
}
.cancel {
  padding: 1em;
}
.cancel button {
  border: none;
  background-color: #ffffff;
  color: hsl(224, 38%, 21%);
  font-weight: 500;
  font-size: 13px;

  text-shadow: 0px 0px 2px hsl(223, 47%, 23%);
}
.cancel button:hover {
  cursor: pointer;
  font-weight: 700;
}
p {
  font-size: 16px;
  color: hsl(224, 23%, 55%)
}
@media only screen and (max-width: 375px) {
  body {
    width: 375px;
    height: auto;
    background-image: url("images/pattern-background-mobile.svg");
    background-repeat: no-repeat;
  }
  .container {
    width: 300px;
    height: auto;
    transform: translate(10%, 10%);
  }
  .container img {
    width: 300px;
    height: auto;
  }
  .container h1 {
    font-size: 20px;
    margin-bottom: 15px;
  }
  .container p {
    width: 200px;
    font-size: 14px;
    text-align: center;
    margin: 0 0 0 50px;
    line-height: 1.5;
  }
  .selector {
    width: 260px;
    height: 70px;
    margin: 0 auto;
    margin-top: 25px;
  }
  .selector img {
    width: 50px;
    left: 8px;
    top: 10px;
    bottom: 5px;
    padding-right: 30px;
  }
  .selector h3 {
    padding: 0;
    font-size: 13px;
    bottom: 20px;
    right: 10px;
  }
  .selector .price{
    font-size: 15px;
    top: 0px;
    right: 84px;
    margin: 0 10px 0 0;
  }
  .selector a {
    right: 15px;
    bottom: 30px;
  }
  .proceed button {
    width: 260px;
    font-size: 11px;
    padding: 15px 50px 15px 50px;
    font-weight: 900;
  }
  .cancel button {
    padding-bottom: 10px;
  }
}


.attribution { 
  font-size: 11px; text-align: center;
  margin-top: 100px; 
}
.attribution a { color: hsl(228, 45%, 44%); }
```

### Continued development

I learned how to do things before starting write a code and some reserch do better and good looking website and responsive

### Useful resources

- [Example resource 1](https://www.w3schools.com/) - This helped me for XYZ reason. I really liked this pattern and will use it going forward.

## Author

- Frontend Mentor - [@Asif_Lopz](https://www.frontendmentor.io/profile/Asif-lopz)
- Twitter - [@Asif_lopz](https://twitter.com/Asif_lopz)

## Acknowledgments

I Thank frontendmentor 


