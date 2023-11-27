## Javascript

#### Q1. Which statement is the correct way to create a variable called rate and assign it the value 100? [R]

- [x] `let rate = 100;`
- [ ] `let 100 = rate;`
- [ ] `100 = let rate;`
- [ ] `rate = 100;`

[Reference Javascript Assignment operators](https://www.w3schools.com/js/js_operators.asp)

#### Q2. How does a function create a closure? [R]

- [ ] It reloads the document whenever the value changes.
- [x] It returns a reference to a variable in its parent scope.
- [ ] It completes execution without returning.
- [ ] It copies a local variable to the global scope.

[Reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Closures)

#### Q3. Which statement creates a new function called discountPrice? [R]

- [x] `A`

```js
let discountPrice = function (price) {
  return price * 0.85;
};
```

- [ ] `B`

```js
let discountPrice(price) {
  return price * 0.85;
};
```

- [ ] `C`

```js
let function = discountPrice(price) {
  return price * 0.85;
};
```

- [x] `D`

```js
discountPrice = function (price) {
  return price * 0.85;
};
```

[Reference defining javascript functions](https://www.w3schools.com/js/js_functions.asp)

#### Q4. Why might you choose to make your code asynchronous? [R]

- [x] to start tasks that might take some time without blocking subsequent tasks from executing immediately
- [ ] to ensure that tasks further down in your code are not initiated until earlier tasks have completed
- [ ] to make your code faster
- [ ] to ensure that the call stack maintains a LIFO (Last in, First Out) structure

**EXPLANATION:**
To ensure that tasks further down in your code are not initiated until earlier tasks have completed" you use the normal (synchronous) flow where each command is executed sequentially. Asynchronous code allows you to break this sequence: start a long running function (AJAX call to an external service) and continue running the rest of the code in parallel.

#### Q5. What is the value of dessert.type after executing this code? [U]

```js
const dessert = { type: 'pie' };
dessert.type = 'pudding';
```

- [ ] pie
- [ ] The code will throw an error.
- [x] pudding
- [ ] undefined

[Reference working with js objects](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Working_with_Objects)

#### Q6. What is the result in the console of running the code shown? [U]

```js
var start = 1;
function setEnd() {
  var end = 10;
}
setEnd();
console.log(end);
```

- [ ] 10
- [ ] 0
- [x] ReferenceError
- [ ] undefined

[Reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Closures)

#### Q7. What will be logged to the console? [U]

```js
console.log('I');
setTimeout(() => {
  console.log('love');
}, 0);
console.log('Javascript!');
```

- [x] .

```plaintext
I
Javascript!
love
```

- [ ] .

```plaintext
love
I
Javascript!
```

- [ ] The output may change with each execution of code and cannot be determined.

- [ ] .

```plaintext
I
love
Javascript!
```

**Reference**
https://developer.mozilla.org/en-US/docs/Web/API/setTimeout#reasons_for_delays_longer_than_specified especially see the 'late timeouts' section.

#### Q8. What is the difference between the `map()` and the `forEach()` methods on the Array prototype? [U]

- [ ] There is no difference.
- [ ] The `forEach()` method returns a single output value, whereas the `map()` method performs operation on each value in the array.
- [x] The map() method returns a new array with a transformation applied on each item in the original array, whereas the `forEach()` method iterates through an array with no return value.
- [ ] The `forEach()` method returns a new array with a transformation applied on each item in the original array, whereas the `map()` method iterates through an array with no return value.

1. [Reference map](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Map)
2. [Reference Differences between forEach and for loop](https://www.geeksforgeeks.org/difference-between-foreach-and-for-loop-in-javascript/)

#### Q9. Given this code, which statement will be evaluated as false? [U]

```js
const a = { x: 1 };
const b = { x: 1 };
```

- [ ] `a['x'] === b['x']`
- [ ] `a != b`
- [x] `a === b`
- [ ] `a.x === b.x`

[Reference](http://adripofjavascript.com/blog/drips/object-equality-in-javascript.html)

[Reference what is use strict in js](https://www.w3schools.com/js/js_strict.asp)

#### Q10. What will this code print? [A]

```js
var v = 1;
var f1 = function () {
  console.log(v);
};

var f2 = function () {
  var v = 2;
  f1();
};

f2();
```

- [ ] 2
- [x] 1
- [ ] Nothing - this code will throw an error.
- [ ] undefined

[Reference closures in js \/ nested functions](https://javascript.info/closure)

#### Q11. The following program has a problem. What is it? [A]

```js
var a;
var b = (a = 3) ? true : false;
```

- [x] The condition in the ternary is using the assignment operator.
- [ ] You can't define a variable without initializing it.
- [ ] You can't use a ternary in the right-hand side of an assignment operator.
- [ ] The code is using the deprecated var keyword.

[Reference ternary operator js](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Conditional_Operator)

#### Q12. You've written the event listener shown below for a form button, but each time you click the button, the page reloads. Which statement would stop this from happening? [A]

```js
button.addEventListener(
  'click',
  function (e) {
    button.className = 'clicked';
  },
  false,
);
```

- [ ] `e.blockReload();`
- [ ] `button.preventDefault();`
- [ ] `button.blockReload();`
- [x] `e.preventDefault();`

[Reference events in javascript](https://developer.mozilla.org/en-US/docs/Web/API/Event/preventDefault)

#### Q13. What is the output that is printed when the div containing the text "Click Here" is clicked? [A]

```html
//HTML Markup
<div id="A">
  <div id="B">
    <div id="C">Click Here</div>
  </div>
</div>
```

```js
//JavaScript
document.querySelectorAll('div').forEach((e) => {
  e.onclick = (e) => console.log(e.currentTarget.id);
});
```

- [x] C B A
- [ ] A
- [ ] C
- [ ] A B C

1. [Reference query selector](https://developer.mozilla.org/en-US/docs/Web/API/Document/querySelector)
2. [Reference events](https://developer.mozilla.org/en-US/docs/Web/Events)

#### Q14. What will this code log to the console? [A]

```js
const myNumbers = [1, 2, 3, 4, 5, 6, 7];
const myFunction = (arr) => {
  return arr.map((x) => x + 3).filter((x) => x < 7);
};
console.log(myFunction(myNumbers));
```

- [ ] `[4,5,6,7,8,9,10]`
- [ ] `[4,5,6,7]`
- [ ] `[1,2,3,4,5,6]`
- [x] `[4,5,6]`

[Reference functions in javascript](https://www.w3schools.com/js/js_functions.asp)

#### Q15. Which statement can be used to select the element from the DOM containing the text "The LinkedIn Learning library has great JavaScript courses" from this markup? [A]

```html
<h1 class="content">LinkedIn Learning</h1>
<div class="content">
  <span class="content">The LinkedIn Learning library has great JavaScript courses!</span>
</div>
```

- [ ] document.querySelector("div.content")
- [x] document.querySelector("span.content")
- [ ] document.querySelector(".content")
- [ ] document.querySelector("div.span")

#### Q16. What will be the value of `result` after running this code? [A]

```js
const person = { name: 'Dave', age: 40, hairColor: 'blue' };
const result = Object.keys(person).map((x) => x.toUpperCase());
```

- [ ] It will throw a TypeError.
- [ ] `["Name", "Age", "HairColor"]`
- [ ] `["DAVE", 40, "BLUE"]`
- [x] `["NAME", "AGE", "HAIRCOLOR"]`

1. [Reference Object.keys()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/keys)
2. [Reference Array.prototype.map()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map)
3. [Reference String.prototype.toUpperCase()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/toUpperCase)

#### Q17. How can you attempt to access the property `a.b` on `obj` without throwing an error if a is undefined? [R]

```js
let obj = {};
```

- [ ] `obj?.a.b`
- [x] `obj.a?.b`
- [ ] `obj[a][b]`
- [ ] `obj.?a.?b`

[Reference Optional chaining (?.)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Optional_chaining)

#### Q18. How would you change the color of this header to pink? [A]

```javascript
<h2 id="cleverest">girls</h2>
```

- [ ] document.getElementByName("cleverest").style.color = "pink";
- [ ] document.getElementsByTagName("h2").style.color = "pink";
- [ ] document.getElementByName("h2").style.color = "pink";
- [x] document.getElementById("cleverest").style.color = "pink";

[Reference: W3Schools HTML DOM Style color Property](https://www.w3schools.com/jsref/prop_style_color.asp)

#### Q19. Which line is missing from this code if you expect the code to evaluate to true? [A]

```js
var compare = function (test1, test2) {
  // Missing line
};

compare(1078, '1078'); // yields true
```

- [ ] `test1==test2;`
- [ ] return test1===test2;
- [x] return test1==test2;
- [ ] return test1!=test2;

[Reference: MDN Equality Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Equality)

#### Q20. What will be logged to the console? [A]

```js
const foo = () => console.log('First');
const bar = () => setTimeout(() => console.log('Second'), 0);
foo();
bar();
console.log('Third');
```

- [ ] Second, First, Third
- [x] First, Third, Second
- [ ] First, Second, Third
- [ ] Third, First, Second
