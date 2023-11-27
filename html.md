## HTML

#### Q1. What is the best way to apply bold styling to text? [R]

- [x] `<strong>`
- [ ] Use CSS.
- [ ] `<bold>`
- [ ] `<b>`

#### Q2. What is the use of the `<link>` tag? [R]

- [ ] when linking style sheets, JavaScript, and icons for mobile apps
- [x] when linking style sheets, favicons, and preloading assets
- [ ] when linking one webpage to another
- [ ] when linking style sheets, external URLs, and favicons

#### Q3. What is the difference between the post and get methods in a form? [U]

- [ ] post is used for sending information to the server. get is used for retrieving form information from the server.
- [ ] get is used for sending information to the server. post is used for retrieving form information from the server.
- [ ] With get, data is included in the form body when sent to the server. With the post, the data goes through the URL.
- [x] With post, data is included in the form body when sent to the server. With get, the data goes through the URL.


#### Q4. In the code below, what is the purpose of the **id** attribute? [U]

```HTML
<p id="warning">Be careful when installing this product.</p>
```

- [x] It establishes that id is a unique identifier in the document, used for styling CSS, scripting, and linking within a webpage.
- [ ] It establishes that id is a unique identifier in the document, used for styling CSS and with Javascript code.
- [ ] It establishes that id may be used for styling CSS several times per page.
- [ ] It establishes that id is a unique identifier in the website, used for styling CSS, scripting, and linking within a webpage.

#### Q5. What is the best semantic markup for the sentence shown? [A]

```
On July 21, 1969, Neil Armstrong said, "One small step for man, one giant leap for mankind."
```

- [x] A

```HTML
<p>
  On <time datetime="1969-07-21">July 21, 1969</time>, Neil Armstrong said,
  <q cite="https://www.hq.nasa.gov/alsj/a11l/a11.html"
    >One small step for man, one giant leap for mankind.</q
  >
</p>
```

- [ ] B

```HTML
<p>
  On July 21, 1969, Neil Armstrong said,
  <q cite="https://www.hq.nasa.gov/alsj/a11l/a11.html"
    >"One small step for man, one giant leap for mankind."</q
  >
</p>
```

- [ ] C

```HTML
<p>
  On July 21, 1969, Neil Armstrong said,
  <q>"One small step for man, one giant leap for mankind."</q>
</p>
```

- [ ] D

```HTML
<p>
  On <time datetime="07-21-1969">July 21, 1969</time>, Neil Armstrong said,
  <q cite="https://www.hq.nasa.gov/alsj/a11l/a11.html"
    >One small step for man, one giant leap for mankind.</q
  >
</p>
```

#### Q6. What is the best way to code three choices within a form so that the user can select only one item? [A]

- [ ] A

```HTML
<label for="example">Make a choice:</label>
<datalist id="example">
  <option value="Choice 1"></option>
  <option value="Choice 2"></option>
  <option value="Choice 3"></option>
</datalist>
```

- [ ] B

```HTML
<p>Make a choice:</p>
<input id="choices" name="example" />

<datalist value="choices">
  <option value="Choice 1"></option>
  <option value="Choice 2"></option>
  <option value="Choice 3"></option>
</datalist>
```

- [ ] C

```HTML
<label for="example">Make a choice:</label>
<input list="example" id="choices" name="choices" />

<datalist id="choices">
  <option value="Choice 1">Choice 1</option>
  <option value="Choice 2">Choice 2</option>
  <option value="Choice 3">Choice 3</option>
</datalist>
```

- [x] D

```HTML
<label for="example">Make a choice:</label>
<input list="choices" id="example" name="example" />

<datalist id="choices">
  <option value="Choice 1"></option>
  <option value="Choice 2"></option>
  <option value="Choice 3"></option>
</datalist>
```

#### Q7. What does the code shown below accomplish? [U]

```html
<picture>
  <source srcset="image1.jpg" media="(min-width: 1000px)" />
  <source srcset="image2.jpg" media="(min-width: 750px)" />
  <img src="image3.jpg" />
</picture>
```

- [x] It displays image1.jpg at 1000px and higher, image2.jpg at 750-999px, and image3.jpg at 749px and lower.
- [ ] It displays image1.jps at 1000px and higher and image2.jpg at 750-999px, image3.jpg is a default in case `<picture>` is not supported.
- [ ] It displays image1.jpg at 1000px and higher and image2.jpg at 750px and higher, image3.jpg is a default in case `<picture>` is not supported.
- [ ] It displays image1.jpg, image2.jpg and image3.jpg at 1000px and higher.

[Source: HTML &lt;picture> Tag](https://www.w3schools.com/tags/tag_picture.asp)

#### Q8. Which HTML snippet links back to the very top of a webpage? [A]

- [x] A

```HTML
<a id="top"></a>

<!-- placed at the top of the page -->

<a href="#top">back to top</a>
```

- [ ] B

```HTML
<a name="top"></a>

<!-- placed at the top of the page -->

<a href="#top">back to top</a>
```

- [ ] C

```HTML
<a href="#">back to top</a> <a href="#top">back to top</a>
```

- [ ] D

```HTML
<button href="#">back to top</button> <button href="#top">back to top</button>
```

#### Q9. What does the `<label>` element do? [U]

- [ ] It labels webpages with important information.
- [ ] It creates an ID for a corresponding input element.
- [ ] It overrides the name attribute's value on a child input element.
- [x] It programmatically associates a text label with an interface element.

#### Q10. To get a link to open in a new window or tab, use the **\_** attribute [R]

- [x] `_blank`
- [ ] `_self`
- [ ] `_new`
- [ ] `_parent`

#### Q11. What is the correctly nested markup for this list? [A]

![Sample list](https://github.com/Ebazhanov/linkedin-skill-assessments-quizzes/blob/main/html/images/ss-6.png?raw=true)

- [ ] A

```HTML
<ul>
  <li>
    office
    <ol style="circle">
      <li>staple</li>
      <li>paper</li>
    </ol>
  </li>
  <li>
    groceries
    <ol style="circle">
      <li>milk</li>
    </ol>
  </li>
</ul>
```

- [x] B

```HTML
<ul>
  <li>
    Office Supplies
    <ul>
      <li>Stapler</li>
      <li>Paper clips</li>
    </ul>
  </li>
  <li>
    Groceries
    <ul>
      <li>Milk</li>
    </ul>
  </li>
</ul>
```

- [ ] C

```HTML
<ul>
  <li>office</li>
  <li>staple</li>
  <li>paper</li>
  <li>groceries</li>
  <li>milk</li>
</ul>
```

#### Q12. What does this code do?

```html
<audio controls>
  <source src="sound.mp3" type="audio/mpeg" />
  <source src="sound.ogg" type="audio/ogg" />
  <source src="sound.wav" type="audio/wav" />
</audio>
```

- [x] The browser chooses the first supported format to play with the browser's default controls.
- [ ] The browser chooses the best audio format to play with JavaScript-provided controls.
- [ ] The browser plays each sound file in order automatically. The user has controls to stop playback.
- [ ] The browser chooses the first supported sound file and will loop the sound until the user stops it.

#### Q13. What is the correct way to code a link that, when clicked, will send an email to `email@example.com` with the subject of "Hello"? [R]

- [ ] `<a href="mailto:email@example.com&subject=Hello">Click me</a>`
- [ ] `<a href="mailto:email@example.com">Hello</a>`
- [x] `<a href="mailto:email@example.com?subject=Hello">Click me</a>`
- [ ] `<a href="mailto:email@example.com?&subject=Hello">Click me</a>`

#### Q14. Which form is coded correctly? [U]

- [ ] A

```HTML
<form>
  <legend>Title</legend>
  <fieldset>
    <label for="name">Your name:</label>
    <input type="text" name="name" id="name" />
    <button type="submit">Submit</button>
  </fieldset>
</form>
```

- [ ] B

```HTML
<form>
  <fieldset>
    <legend>Title</legend>
    <p>Your name:</p>
    <input type="text" name="name" id="name" />
    <input type="submit" value="Submit" />
  </fieldset>
</form>
```

- [x] C

```HTML
<form>
  <fieldset>
    <legend>Title</legend>
    <label for="name">Your name:</label>
    <input type="text" name="name" id="name" />
    <button type="submit">Submit</button>
  </fieldset>
</form>
```

- [ ] D

```HTML
<form>
  <legend>Title</legend>
  <label for="name">Your name:</label>
  <input type="text" name="name" id="name" />
  <input type="submit" value="Submit" />
</form>
```

#### Q15. What does the **poster** attribute do in the `<video>` tag? [R]

- [x] It specifies an image that should be displayed while the video downloads and until the video is played.
- [ ] It specifies an image that only displays if there is a problem with the video.
- [ ] It specifies an image that should be displayed until the video is played.
- [ ] It specifies an image that should be displayed while the video downloads.

#### Q16. What does this code do? [R]

```HTML
<audio controls src="sound.mp3" type="audio/mpeg">When does this text display?</audio>
```

- [ ] The text displays over the audio controls unless CSS is used to position it elsewhere.
- [ ] The text displays under the audio controls.
- [x] The text displays when the browser cannot play the sound.
- [ ] The text never displays.


#### Q17. Which snippet of HTML, when clicked, makes a phone call on a mobile device? [R]

- [x] `<a href="tel:802-555-1212">Call me</a>`
- [ ] `<a href="phone">802-555-1212</a>`
- [ ] `<a href="tel">802-555-1212</a>`
- [ ] `<a href="phone:802-555-1212">Call me</a>`

#### Q18. What is the purpose of the `class` attribute? [U]

- [ ] Classes allow CSS to select specific elements on the page. You may list as many class names within the class attribute as you wish,
  separated by spaces.
- [ ] Classes allow CSS and JavaScript to select specific elements on the page. You may list only one class name per class attribute.
- [ ] Classes allow CSS to select specific elements on the page. You may list only one class name per class attribute.
- [x] Classes allow CSS and JavaScript to select specific elements on the page. You may list as many class names within the class attribute
  as you wish, separated by spaces.

[Reference (MDN)](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes/class)


#### Q19. What is the most semantically accurate way to make up a main navigation bar, displayed in a horizontal direction? [A]

- [ ] A

```html
<p>
  <a href="index.html">Home</a>
  <a href="about.html">About</a>
  <a href="contact.html">Contact</a>
</p>
```

- [ ] B

```html
<nav>
  <a href="index.html">Home</a>
  <a href="about.html">About</a>
  <a href="contact.html">Contact</a>
</nav>
```

- [ ] C

```html
<nav>
  <ol>
    <li><a href="index.html">Home</a></li>
    <li><a href="about.html">About</a></li>
    <li><a href="contact.html">Contact</a></li>
  </ol>
</nav>
```

- [x] D

```html
<nav>
  <ul>
    <li><a href="index.html">Home</a></li>
    <li><a href="about.html">About</a></li>
    <li><a href="contact.html">Contact</a></li>
  </ul>
</nav>
```

#### Q20. In which order will these scripts execute, assuming they all take the same time to download? [R]

```HTML
<script type="module" src="module.js"></script>
// external module
<script type="async" src="module.js"></script>
// async
<script type="defer" src="module.js"></script>
// defer
<script type="module" src="module.js">
  // inline module
</script>
```

- [ ] async, external module, defer, inline module
- [ ] async, inline module, external module, defer
- [x] external module, async, defer, inline module
- [ ] inline module, external module, defer, async
