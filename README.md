To use ink, add this script to your HTML:

     <script src="ink.js" > </script>
     
<hr>

To add a character, create an object with its properties.

	Banana = {
 		type: "image",
 		source: "banana.jpg",
 		width: 25,
 		x: 0,
 		y:0,
	};

      
Next, add the name to the layer list to tell the computer to render it.

     layerList = [ Banana ];

To add functionality, use the forever function to repeat the code indefinitely.

	function forever(){
		Banana.x = mouse.x;
		Banana.y = mouse.y;
	}
     
output:

> [<img src="https://coolprofessor.github.io/ink.js/demo/banana.gif" width="150"/>](https://coolprofessor.github.io/ink.js/demo/)

A full description of this can be found in the [Documentation](https://coolprofessor.github.io/ink.js/documentation).
