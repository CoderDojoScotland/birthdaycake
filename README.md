# Coderdojo Scotland HTML/CSS Cake

**Happy 5th Birthday - Coderdojo Scotland**

![5 Binary Balloon](http://coderdojoscotland.com/balloon.png)

## Getting Started

Fork our Codepen - [https://codepen.io/papertank/pen/yoYJGV](https://codepen.io/papertank/pen/yoYJGV)

or

Download or Fork our Github repository - [https://github.com/CoderDojoScotland/birthdaycake](https://github.com/CoderDojoScotland/birthdaycake)

## About

This simple repository contains HTML and CSS to render a birthday cake, celebrating Coderdojo Scotland's 5th Birthday.

The cake is styled entirely with CSS, using standard properties (like `background` and `border-radius`) as well as more modern properties (such as `animation` and `justify-content`).

## Editing

- The rules near the top of the css affect the width and height of the elements - feel free to play around with these. Just make sure that the height of the `.candle` `.sponge` and `.icing` add up to 100%;
- Fancy a different colour of sponge or icing? Just edit the background colours of those elements in the style.css file. Don't forget that CSS uses the American spelling - `color`!
- Want to slow or speed up the candle flicker? Just change the seconds of the `animation` property.

## Live Reload

Using npm, this repository requires browserSync and gulp for live reload of the HTML and CSS.

1. Make sure you have [npm installed](https://www.npmjs.com/get-npm)
2. Install the dependencies `npm install`
3. Run `gulp watch`
4. Edit the style.css file or index.html and the browser will live reload.

## FAQs

**Why do the div elements use class instead of id?**

Classes are often used in CSS to select elements to apply properties to - classes begin with a dot, so `<div class="cake"></div>` is selected in CSS with `.cake { }`.
IDs can also be used, but they are designed to be used only once per page - for example `<div id="cake"></div>` selected by `#cake { }`.
For more information on the difference, see [https://css-tricks.com/the-difference-between-id-and-class/](https://css-tricks.com/the-difference-between-id-and-class/)

**Why are some of the div elements inside of others, and why are they named like that?**

There are a number of ways the HTML (and CSS) could have been written and organised. Different developers might have used less or more elements on the HTML, used different class names, or used different CSS rules to achieve the exact same appearance.
From a styling point of view, and to match real life, I feel like the `filling` should be inside the `sponge` and the `wick` should be inside the `candle`. Why not try moving the HTML about and changing the CSS to match?

**Why not just use an image of a cake, or a background image for the sponge and icing?**

In this example, because it's fun to see what is possible using some simple CSS. In real life, images have some limitations:

- They are slower to load (for instance on a mobile connection).
- They don't scale as well on different devices.
- It's harder or impossible to change the dimensions without editing the image itself.

**What is display: flex?**

Flexbox (or Flex) is a new CSS module which aims at making layouts and aligning elements much easier in CSS.
In this example, we use the following lines to simply centre the cake in the middle of the page. Without flexbox, this would require strange positioning and negative margins to achieve the same display.

```
display: flex;
align-items: center;
justify-content: center;
```

For more on flexbox, see [https://css-tricks.com/snippets/css/a-guide-to-flexbox/](https://css-tricks.com/snippets/css/a-guide-to-flexbox/).

## Credits

 * [Matthias Martin](https://codepen.io/roydigerhund/pen/qZLBBW) for CSS candle inspiration.
 * [Chris Baldie](http://chrisbaldie.com) for cake design.

## Author

[David Rushton - Papertank](http://papertank.co.uk)

# License

[MIT License](https://github.com/CoderDojoScotland/birthdaycake/blob/master/LICENSE)
