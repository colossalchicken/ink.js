Ink.js is an object-oriented tool for creating online apps and games. It is simple, and does not require any installation.
<br><br>
To use ink, add this script to your HTML:

     <script src="https://ink.js.org/ink.min.js" > </script>

<hr><br>
To add a character, create an object with its properties.

    Banana = {
    	type: "image",
		source: "https://ink.js.org/demo/banana.jpg",
 		width: 25,
 		x: 0,
 		y:0,
    };


<br>

> Ink.js only notices an object if it has a `type` or `contents` property. 
> To change how the characters overlap, use `layerList`.

<br>

To add functionality, use the forever function to repeat the code indefinitely.

	function forever(){
		Banana.x = mouse.x;
		Banana.y = mouse.y;
	}
     
output:

> <a href="https://coolprofessor.github.io/ink.js/demo/"><img src="https://ink.js.org/demo/banana.gif" width="150" /></a>

A full description of this can be found in the [wiki](https://github.com/coolprofessor/ink.js/wiki#welcome-to-the-inkjs-wiki).
<br>
> This site is in no way related to [ink.sapo.pt](https://ink.sapo.pt).
