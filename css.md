## CSS

#### Q1. Using an attribute selector, how would you select an `<a>` element with a "title" attribute? [A]

- [x] `a[title]{...}`
- [ ] `a > title {...}`
- [ ] `a.title {...}`
- [ ] `a=title {...}`

#### Q2. CSS grid introduced a new length unit, fr, to create flexible grid tracks. Referring to the code sample below, what will the widths of the three columns be? [U]

```css
.grid {
  display: grid;
  width: 500px;
  grid-template-columns: 50px 1fr 2fr;
}
```

- [ ] The first column will have a width of 50px. The second column will be 50px wide and the third column will be 100px wide.
- [x] The first column will have a width of 50px. The second column will be 150px wide and the third column will be 300px wide.
- [ ] The first column will have a width of 50px. The second column will be 300px wide and the third column will be 150px wide.
- [ ] The first column will have a width of 50px. The second column will be 500px wide and the third column will be 1000px wide.

#### Q3. There are many properties that can be used to align elements and create page layouts such as float, position, flexbox, and grid. Of these four properties, which one should be used to align a global navigation bar that stays fixed at the top of the page? [A]

- [x] position
- [ ] flexbox
- [ ] grid
- [ ] float

#### Q4. When elements overlap, they are ordered on the z-axis (i.e., which element covers another). The z-index property can be used to specify the z-order of overlapping elements. Which set of statements about the z-index property are true? [R]

- [x] Larger z-index values appear on top of elements with a lower z-index value. Negative and positive numbers can be used. z-index can only be used on positioned elements.
- [ ] Smaller z-index values appear on top of elements with a larger z-index value. Negative and positive numbers can be used. z-index must also be used with positioned elements.
- [ ] Larger z-index values appear on top of elements with a lower z-index value. Only positive numbers can be used. z-index must also be used with positioned elements.
- [ ] Smaller z-index values appear on top of elements with a larger z-index value. Negative and positive numbers can be used. z-index can be used with or without positioned elements.

#### Q5. What are three valid ways of adding CSS to an HTML page? [R]

- [ ] A

```
  1. External; CSS is written in a separate file.
  2. Inline; CSS is added to the <head> of the HTML page.
  3. Internal; CSS is included within the HTML tags.
```

- [ ] B

```
  1. External; CSS is written in a separate file and is linked within the <header> element of the HTML file.
  2. Inline; CSS is added to the HTML tag.
  3. Internal; CSS is included within the <header> element of the HTML file.
```

- [ ] C

```
  1. External; CSS is written in a separate file and is linked within the <head> element of the HTML file.
  2. Internal; CSS is included within the <header> element of the HTML file.
  3. Inline; CSS is added to the HTML tag.
```

- [x] D

```
  1. External; CSS is written in a separate file and is linked within the <head> element of the HTML file.
  2. Inline; CSS is added to the HTML tag.
  3. Internal; CSS is included within the <head> element of the HTML file.
```

#### Q6. In the example below, when will the color pink be applied to the anchor element? [R]

```css
a:active {
  color: pink;
}
```

- [ ] The color of the link will display as pink after it has been clicked or if the mouse is hovering over the link.
- [ ] The color of the link will display as pink on mouse hover.
- [x] The color of the link will display as pink while the link is being clicked but before the mouse click is released.
- [ ] The color of the link will display as pink before it has been clicked.

#### Q7. How would you make the first letter of every paragraph on the page red? [A]

- [x] p::first-letter { color: red; }
- [ ] p:first-letter { color: red; }
- [ ] first-letter::p { color: red; }
- [ ] first-letter:p { color: red; }

#### Q8. In this example, what is the selector, property, and value? [R]

```css
p {
  color: #000000;
}
```

- [ ] A

```
  "p" is the selector
  "#000000" is the property
  "color" is the value
```

- [x] B

```
  "p" is the selector
  "color" is the property
  "#000000" is the value
```

- [ ] C

```
  "color" is the selector
  "#000000" is the property
  "#p" is the value
```

- [ ] D

```
  "color" is the selector
  "p" is the property
  "#000000" is the value
```

#### Q9. In the following media query example, what conditions are being targeted? [U]

```css
@media (min-width: 1024px), screen and (orientation: landscape) { … }
```

- [x] The rule will apply to a device that has either a width of 1024px or wider or is a screen device in landscape mode.
- [ ] The rule will apply to a device that has a width of 1024px or narrower and is a screen device in landscape mode.
- [ ] The rule will apply to a device that has a width of 1024px or wider and is a screen device in landscape mode.
- [ ] The rule will apply to a device that has a width of 1024px or narrower or is a screen device in landscape mode.

#### Q10. There are many advantages to using icon fonts. What is one of those advantages? [U]

- [ ] Icon fonts increase accessibility.
- [ ] Icon fonts can be used to replace custom fonts.
- [x] Icon fonts can be styled with typography-related properties such as font-size and color.
- [ ] Icon fonts are also web-safe fonts.

#### Q11. What is the difference between `display:none` and `visibility:hidden`? [R]

- [ ] Both will hide the element on the page, but display:none has greater browser support. visibility:hidden is a new property and does not have the best browser support
- [ ] display:none hides the elements but maintains the space it previously occupied. visibility:hidden will hide the element from view and remove it from the normal flow of the document
- [x] display:none hides the element from view and removes it from the normal flow of the document. visibility:hidden will hide the element but maintain the space it previously occupied.
- [ ] There is no difference; both will hide the element on the page

#### Q12. What is the difference between the margin and padding properties? [U]

- [ ] Margin adds space around and inside of an element; padding adds space only inside of an element.
- [x] Margin adds space around an element; padding adds space inside of an element.
- [ ] Margin adds a line around an element, and padding adds space inside of an element.
- [ ] Margin adds space inside of an element, and padding adds space around an element.

#### Q13. Which style places an element at a fixed location within its container? [R]

- [x] position: absolute;
- [ ] display: flex;
- [ ] display: block;
- [ ] float: left;

#### Q14. The calc() CSS function is often used for calculating relative values. In the example below, what is the specified margin-left value? [R]

```css
.example {
  margin-left: calc(5% + 5px);
}
```

- [x] The left margin value is equal to 5% of its parent element's width plus 5px
- [ ] The left margin value is equal to 5% of the viewport width plus 5px
- [ ] The left margin value is equal to 5% of the closest positioned element's width plus 5px
- [ ] The left margin value is equal to 5% of the selected element's width (.example) plus 5px

#### Q15. When would you use the @font-face method? [R]

- [ ] to set the font size of the text
- [x] to load custom fonts into stylesheet
- [ ] to change the name of the font declared in the font-family
- [ ] to set the color of the text

#### Q16. What is the correct selector for targeting all text inputs that are not disabled? [A]

- [x] `input[type="text"]:not([disabled]) {...}`
- [ ] `input[type="text"]:not("disabled") {...}`
- [ ] `input[type*="text"]:not([disabled="disabled"]) {...}`
- [ ] `input[type="text"]:not([type="disabled"]) {...}`

`input[type="text"]` selects all the input with type text, and `:not([disabled])` select all the elements not having the attribute "disabled". Combining both only selects all the input elements with type attribute as "text" and not having "disabled" attribute.`

1. [Reference link attribute-selector](https://www.w3schools.com/css/css_attribute_selectors.asp)
2. [Reference link-:not()](https://developer.mozilla.org/en-US/docs/Web/CSS/:not)

#### Q17. Using this HTML markup, how would you select only the headings contained within the `<header>` element? [A]

```HTML
<header>
  <h1>Heading 1</h1>
  <h2>Heading 2</h2>
</header>
<h2>Heading 2</h2>
```

- [x] `header h1, header h2 {...}`
- [ ] `header h1 + header h2 {...}`
- [ ] `header h1, h2 {...}`
- [ ] `h1, h2 {...}`

#### Q18. What is the output of the margin value when used within this context, assuming that its containing element is larger than 800px? [A]

```css
.example {
  width: 800px;
  margin: 0 auto;
}
```

- [ ] The example element will have 0 margin space around the whole element. The auto value will center align the element horizontally and vertically within its container.
- [ ] The example element will have 0 margin spaces on the left and right. It will be sized automatically on the top and bottom, which will center align the element within its container.
- [x] The example element will have 0 margin spaces on the top and bottom. The margin will be sized automatically on the left and right, which may center-align the element within its container.
- [ ] The margin value is invalid because it's missing a unit measurement after the 0.

[Source: SOW](https://stackoverflow.com/questions/3170772/what-does-auto-do-in-margin-0-auto)

#### Q19. Which style will horizontally center the inner &lt;div&gt; within the outer &lt;div&gt;? [A]

```js
<div id="outer">
  <div id="inner">Center Me!</div>
</div>
```

- [ ] A

```css
#inner {
  width: 50%;
}

#outer {
  width: 100%;
}
```

- [ ] B

```css
#inner {
  left: 0;
  right: 0;
  position: center;
}
```

- [ ] C

```css
#inner {
  text-align: center;
}
```

- [x] D

```css
#inner {
  width: 50%;
  margin: 0 auto;
}
```

#### Q20. To center the content of a grid cell horizontally and vertically within the cell, which style rule should you apply? [A]

- [ ] A

```css
align-items: start;
justify-items: end;
```

- [x] B

```css
align--items: center;
justify-items: center;
```

- [ ] C

```css
align-items: middle;
justify-items: middle;
```

- [ ] D

```css
align-items: stretch;
justify-items: stretch;
```

[Reference for align-items](https://developer.mozilla.org/en-US/docs/Web/CSS/align-items) [Reference for justify-items](https://developer.mozilla.org/en-US/docs/Web/CSS/justify-items)
