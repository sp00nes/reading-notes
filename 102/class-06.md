# Class 06 Reading Notes *(9/21/22)*

[*back*](../README.md)

## How computers work

Computers Input, store, process, and output

computers use wires turing on and off to represent binary

Programming languages just give you a more intuitive way to write code in something closer to english.

## Java Script

We can distinguish 3 major parts of what we usually refer to as "JavaScript".

- The language itself. This is fairly standard among the various environments, both in the various browsers and in the various server-side environments.
- The DOM API - how the language can interact with the various parts of a web page while in the browser. While in this respect the various browsers are getting closer to each other they still differ. Several libraries, most prominently JQuery, is trying to provide a unified API.
- The server API (or just API) provided by Node.js or one of the other server-side systems.

you can embedded java directly into an HTML file. or you can connect javascript via remote file.

Alert - makes a pop-up in the browser with text.

``` html
<script language="javascript">
 
alert("Hello World");
 
</script>
```

Document.write - writes text onto the page, can be used to change text.

``` html
First line
<script>
 
document.write("<h1>Hello World</h1>");
 
</script>
Last line
```

console.log - writes message to the JS consol (CTRL + SHIFT + J)

```html
<script>
 
console.log("Hello World");
 
</script>
```

Prompt - creates a textbox that has an input option for the user

```html
<script>
 
var name = prompt("Your name:", "");
document.write("Hello ", name);
 
</script>
```

``` html
<script>
 
var name = prompt("Please correct your e-mail address:", "foo@bar.co");
document.write("Your e-mail address is ", name);
 
</script>
```

Confirm - asks the user a yes or no question. (ok/cancel)

``` html
<script>
 
if (confirm("Shall I print Hello World?")) {
    document.write("Hello World");
} else {
    document.write("OK, I won't print it.");
}
 
</script>
```
