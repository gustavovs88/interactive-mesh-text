# interactive-mesh-text
An mouse position interactive mesh text code.
## How to use
Download the code from git-hub and have fun changing the attributes in the script.js file to have different designs and responses.
## Main code Attributes
```Javascript
//determine canvas size:
let canvasWidth = canvas.width = 1920;
let canvasHeight = canvas.height = 800;

// Determine the font size to be drawn in the canvas - larger font sizes gives more particles
let fontSize = 30

// Choose the factor for enlarging the font size - Larger factors makes the distance bigger between particles
let fontSizeFactor = 8;

// Adjust the text position:
let positionAdjustX = 0;
let positionAdjustY = 0;

// Change it to the text you want to use:
let text = "Mesh Text";

// Change the action radius of the mouse:
const mouse = {
  x: null,
  y: null,
  radius: 150,
};

// lines 59:73  in the Particle class constructor 
    //-> Change tha particles size
         this.size = Math.random() * 3 + 1;

    //-> Change tha particles density - This is related to the speed wich the particles will move:
         this.density = Math.random() * 30 + 1;

    //-> Change the particles color:
         this.color = `rgb(${Math.floor(Math.random() * 255)}, ${Math.floor(
              Math.random() * 255
            )}, ${Math.floor(Math.random() * 255)}, 1`
  
// line 149 -> change the mesh lines width:
        ctx.lineWidth = Math.random() * 2;
        
// line 159 -> change the max distance between particles wich draws lines to connect particles:
       distance < 20
       
// line 168 -> change the mesh lines color:
        ctx.strokeStyle = `rgb(255,255,255, +${opacityValue})`
```
## Comments
This code does a heavy processing since it uses animation to update each particle and mesh line. If the animation become less fluid, try reduce the number of particles and lines.

## Mention
This code is based in Franks Laboratory youtube channel videos:
https://www.youtube.com/channel/UCEqc149iR-ALYkGM6TG-7vQ
