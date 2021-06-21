>### [Code](https://github.com/coolprofessor/ink.js/blob/main/ink.min.js)   &nbsp;&nbsp;  |  &nbsp;&nbsp;    Editor &nbsp;&nbsp;  | &nbsp; &nbsp; [Github](https://github.com/coolprofessor/ink.js#code-------editor------documentation)


## Documentation
This is the documentation for the Ink.js Program.
The list of features is always growing, so the syntax may change over time.

## Setup 
To begin using ink, create a  HTML file, and add a script like so:

    <script src="https://coolprofessor.github.io/ink.js/ink.min.js" > </script>
    
<br>

There are a lot of good HTML editors. Here is a list of some simple ones:

- [Tryit Editor v3.6 (w3schools.com)](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_default)
- [Tynker](https://www.tynker.com/)

## Basic code
The program is set up with characters, called entities. They are set up in objects, that hold information about them. Here is an Example::

    cow = {
	    type: "image",
	    source: "cow.png",
	    x: 0,
	    y: 0,
	    selectable: false
    }
<br>
The entities are listed in an array called "layerList". This list shows in what order entities overlap.

    layerList = ["cow"]
    
> Note: The characters are listed in string format, so you can easily edit the array with variables.

<br>
To make the program interactive, there is a loop called forever, that repeats a set of code infinitely.

    function forever(){
	    
    }
    
>Note: to change the speed of the loop and rendering, change the `frameDelay` variable (milliseconds) 

<br>
The mouse and keyboard have objects that show their information as well.


    mouse = {
	    x: 540,
	    y: 326,
	    cursor:  "none",
	    down:    function(){},
	    up:      function(){},
	    moved:   function(){},
	    pressed: false,
	    scrool:  function(){};
	    scroolX: 0,
	    srcoolY: 20
    }
    
    key = {
	    name: "c",
	    code: 67,
	    pressed: function(){},
    }
    
    var page = {
		selectable: true,
		editable: false,
		//execute it, don't edit it
		reset: null
	};
<br>
<br>

## entity properties
These are the properties that you can add to an entity.
<br> 

**type**
- This specifies the type of entity. If the type is an image, add a "source" property including the URL. You can also specify the height and width in the object.

- Input: "image", "html", null

- Example: `type: "image"`

<br>

**contents**
- This is the html code for the entity. It is only for html type entities.

- Input: string, number

- Example: `contents: "<p>hi</p>"`

<br>

**position**
- This specifies the position relative to the top left corner of the window.

- Input: number, null

- Example: `x:0, y: 23`

 >Note:  If  both x and y are null, the entity will align to the center.

 <br>

**selectable**
- This property determines if text is selectable or not. It also determines if images are draggable.

- Input: Boolean

- Example: `selectable: false`

<br>

**onclick, onmouseover**
- These functions will be declared when the mouse clicks on the entity or moves on the entity. To execute a function when the mouse is clicked anywhere in the window, use `mouse.down = function(){}`.

- Input: function

- Example: `onclick: function(){}` `onmouseover: function(){}`

<br>

**visible**
- This hides the entity.

- Input: Boolean

- Example: `visible: true`

<br>

**color**
- This changes the color of the entity (CSS)

- Input: string holding CSS color

- Example: `color: "blue"`

<br>

**background-color**
- This changes the background  color of the entity (CSS)

- Input: string holding CSS color

- Example: `background: "blue"`

<br>


**Rotation**

- This changes the rotation of the entity.

- Input: number

- Example: `rotate: 26`

<br>

##  other stuff

**Random**

- This pics a random number between min and max.

- Input: ( min, max )

- Example: `random(-77,55)`

<br>

**copy**

- You can copy text with this tool.

- Input: string

- Example: `rotate: 26`

<br>

**repeat**

- This function is used to repeat code

- Input: number, function

- Example: `repeat(10,function(){ alert("hello") })`
