# Elements

```html
<!-- Format: -->
<element>
  ...content
</element>

<!-- Examples: -->
<h1>This is a large header</h1>

<p>
  This is a paragraph. It can contain as many words as you need.
</p>

<div>
  This is a div, a generic element that contains other elements.
  <h4>Like this smaller header,</h4>
  <p>And this paragraph</p>
</div>
```

__HTML Elements__ (AKA HTML Tags) are the objects we place within an HTML __document__.

They are specific words wrapped in angle brackets (`<` and `>`).
We say that they are _opened_ when you write a tag, (ie. `<header>`),
and _closed_ when you  right the tag again, this time with a forward slash (ie. `</header>`.

## Block Elements

```html
<h1>The header of my documents</h1>
<h4>The subheader; a bit of context</h4>

<p>
  This is where I describe what my page is about.
  Paragraphs are generally much longer than headers.
</p>
```

By default, __Block Elements__ take up the entire width of the document.

In the example to the right, each element will be on its own horizontal section.

<a target="_blank" href="http://codepen.io/bwt604RED/pen/evMgoK">View in Codepen</a>

## Inline Elements

```html
<p>
  <strong>This strong text</strong>
  is beside this normal text
  <em>and beside this emphasized text</em>
</p>

<div>
  <!-- These images will be beside each other -->
  <img src="http://placehold.it/150x150" alt="First image">
  <img src="http://placehold.it/150x150" alt="Second image">
  <img src="http://placehold.it/150x150" alt="Third image">  
</div>
```

Unlike Block Elements, __Inline Elements__ are displayed _in a line_.

<a target="_blank" href="http://codepen.io/bwt604RED/pen/evMgwK">View in Codepen</a>


## Void Elements

```html
<!-- Void Element Usage -->
<img src="http://placehold.it/150x150" alt="First image">
<br>
<input type="text" name="myInput">
```

__Void__ (AKA Empty) elements are not designed to have any content.
Because of this, they don't require a closing tag.

<a target="_blank" href="http://codepen.io/bwt604RED/pen/NpYdQj">View in Codepen</a>


## Reference

```html
<!-- List examples -->
<ol>
  <li>This will be an ordered (numbered) list</li>
  <li>You can have as many items as you need</li>
</ol>

<ul>
  <li>This will be an unordered (bullet) list</li>
  <li>You can have as many items as you need</li>
</ul>

<!-- Grouping Examples -->
<div>
  DIV elements are used for grouping elements. You can add text...
  <p>
    But it is usually better to add text within
    <em>typography elements</em>
    like paragraphs.
  </p>
</div>

<header>
  HTML5 gave us more semantic elements like <em>Header</em>.
  It acts the same as div, but its name gives us an idea of what it <em>does</em>.

  <ul class="menu">
    <li>Home</li>
    <li>About</li>
    <li>Pricing</li>
    <li>Contact</li>
  </ul>
</header>

<!-- Form Example -->
<form>
  <label for="username">Username</label>
  <input type="text" id="username"> <br>

  <label for="password">Password</label>
  <input type="password" id="password"> <br>

  <select>
    <option value="volvo">Volvo</option>
    <option value="saab">Saab</option>
    <option value="mercedes">Mercedes</option>
    <option value="audi">Audi</option>
  </select> <br>

  <label for="description">Description</label> <br>
  <textarea id="description"></textarea>
</form>

<!-- Media Examples -->
<img src="http://placehold.it/150x150" alt="Second image">

<audio controls>
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
  Your browser does not support the audio tag.
</audio>

<video width="320" height="240" controls>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
  Your browser does not support the video tag.
</video>
```

Here are some of the more common elements and their usage.
There are many more, but this should get you started!

<a target="_blank" href="http://codepen.io/bwt604RED/pen/vxRxBO">View Examples in Codepen</a>

__Typography__

| Element | Example | Type | Void |
|---------|---------|------|------|
|Heading 1|`<h1>Main Heading</h1>`|Block|False|
|Heading 2|`<h2>Secondary Heading</h2>`|Block|False|
|Heading 3|`<h3>Smaller than h2</h3>`|Block|False|
|Heading 4|`<h4>Smaller than h3</h4>`|Block|False|
|Heading 5|`<h5>Smaller than h4</h5>`|Block|False|
|Heading 6|`<h6>Smaller than h5</h6>`|Block|False|
|Paragraph|`<p>This is where we place regular text</p>`|Block|False|
|Strong|`<p>One word will be <strong>bold</strong></p>`|Inline|False|
|Emphasis|`<p>One word will be <em>emphasized</em></p>`|Inline|False|
|Span|`<p>One word can be <span>styled</span></p>`|Inline|False|
|Line Break|`<p>This will be on <br> 2 lines</p>`|Inline|True|

__Lists__

| Element | Example | Type | Void |
|---------|---------|------|------|
|Ordered List|`<ol></ol>`|Block|False|
|Unordered List|`<ul></ul>`|Block|False|
|List Item|`<li></li>`|Block|False|

__Grouping__

| Element | Example | Type | Void |
|---------|---------|------|------|
|Header|`<header></header>`|Block|False|
|Footer|`<footer></footer>`|Block|False|
|Division|`<div></div>`|Block|False|
|Section|`<section></section>`|Block|False|
|Article|`<article></article>`|Block|False|

__Forms__

| Element | Example | Type | Void |
|---------|---------|------|------|
|Form|`<form></form>`|Block|False|
|Input|`<input>`|Inline|True|
|Dropdown Menu (Select)|`<select></select>`|Inline|False|
|Dropdown Menu Option|`<option></option>`|Inline|False|
|Large Text Box|`<textarea></textarea>`|Inline|False|
|Input Label|`<label></label>`|Inline|False|
|Button|`<button></button>`|Inline|False|

__Media__

| Element | Example | Type | Void |
|---------|---------|------|------|
|Image|`<img>`|Inline|True|
|Audio|`<audio></audio>`|Block|False|
|Video|`<video></video>`|Block|False|







