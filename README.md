# Ink.js
Ink.js is a tool that thinks outside the box, figuratively and literaly. Insted of using the canvas, ink.js uses HTML elements to render content. It is an object-oriented, simple, and does not require any installation.
<br><br>
To use ink, add this script to the top of your HTML:

```html
<script src="https://ink.js.org/ink.min.js" ></script>
```
<br>
To add a character, create an object with its properties.

```javascript
Banana = {
    type: "image",
    source: "https://ink.js.org/demo/banana.jpg",
    width: 25,
    x: 0,
    y:0,
};
```
<br>

> Ink.js only notices an object if it has a `type` or `contents` property. 
> To change how the characters overlap, use `layerList`.

<br>

To add functionality, use the forever function to repeat the code indefinitely.

```javascript
forever = ()=>{
	Banana.x = mouse.x;
	Banana.y = mouse.y;
}
```
output:

> [![click to open](https://ink.js.org/demo/banana.gif)](https://coolprofessor.github.io/ink.js/demo/)
