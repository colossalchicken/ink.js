# Character Properties
Ink.js reads objects and creates HTML elements out of them. Here are the possible properties.

**type** ***(not required)*** **:** This specifies the type of character. If the type is an image, add a "source" property including the URL.
<br>**contents:** This is the html code for the character. Example: `contents: "<p>hi</p>"`

name | input |example
--- | --- | ---
x | int | `x: 0`
y | int | `y: 0`
width | int | `width: 50`
height | int | `height: 100`
selectable|bool| `selctable: false`
onclick | func | `onclick: ()=>{alert('ouch!')}`
onmouseover | func | `onmouseover: ()=>{alert('hi!')}`
mousedown | func | `mousedown: ()=>{alert('hello!')}`
mouseup | func | `mouseup: ()=>{alert('bye!')}`
visible | bool | `vivsible : false`
color | str | `color: 'blue'` ***(use CSS)***
backgorund | str | `background: 'red'` ***(use CSS)***
rotation | int | `rotate: 90`

