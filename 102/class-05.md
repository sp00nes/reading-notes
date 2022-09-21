# Class 05 Reading Notes *(9/21/22)*

[*back*](../README.md)

## CSS

HTML is the skeleton and the bones, CSS is the clothes and makeup. CSS (Cascading Style Sheets) can be used to change basic document text styling or it can be used to create a layout.

CSS is a rule-based language you define the rules by specifying groups of styles that should be applied to particular elements or groups of elements on your web page.

- In the above example, the CSS rule opens with a selector. This selects the HTML element that we are going to style. In this case, we are styling level one headings (\<h1\>).
- We then have a set of curly braces { }.
- Inside the braces will be one or more declarations, which take the form of property and value pairs. We specify the property (color in the above example) before the colon, and we specify the value of the property after the colon (red in this example).

All web standards technologies (HTML, CSS, JavaScript, etc.) are defined in giant documents called specifications (or "specs"), which are published by standards organizations (such as the W3C, WHATWG, ECMA, or Khronos) and define precisely how those technologies are supposed to behave. CSS is no different — it is developed by a group within the W3C called the CSS Working Group

- The CSS element Selector
  - The element selector selects HTML elements based on the element name.

``` css
p {
  text-align: center;
  color: red;
}
```

- The CSS id Selector
  - The id selector uses the id attribute of an HTML element to select a specific element. The id of an element is unique within a page, so the id selector is used to select one unique element! To select an element with a specific id, write a hash (#) character, followed by the id of the element.

``` css
#para1 {
  text-align: center;
  color: red;
}
```

``` HTML
<p id="para1">Hello World!</p>
```

- The CSS class Selector
  - The class selector selects HTML elements with a specific class attribute. To select elements with a specific class, write a period (.) character, followed by the class name.
  
``` css
.center {
  text-align: center;
  color: red;
}
```

You can also specify that only specific HTML elements should be affected by a class.

``` css
p.center {
  text-align: center;
  color: red;
}
```

``` html
<p class="center large">This paragraph refers to two classes.</p>
```

- The CSS Universal Selector
  - The universal selector (*) selects all HTML elements on the page.

``` css
* {
  text-align: center;
  color: blue;
}
```

- The CSS Grouping Selector
  - The grouping selector selects all the HTML elements with the same style definitions.

``` css
h1 {
  text-align: center;
  color: red;
}

h2 {
  text-align: center;
  color: red;
}

p {
  text-align: center;
  color: red;
}
```

``` css
h1, h2, p {
  text-align: center;
  color: red;
}
```

[CSS Reference](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference)

[CSS Style Reset](https://meyerweb.com/eric/tools/css/reset/)
