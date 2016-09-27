#draggable Shapes

This is a library for making 2d shapes that are easy to move around within p5.js. It uses the <a href="https://github.com/bmoren/p5.collide2D">2dCollide</a> library as well.

##Setup
- Download the p5.draggableShape.js and p5.2dcollide.js files and add them to you sketch's libraries
- Link the libraries in the html in your p5 project folder. 
- You're good to go.

You can find out more about installing p5 libraries <a href="https://github.com/processing/p5.js/wiki/Libraries#adding-a-library-to-your-project">here</a>.

##Usage
```javascript
var circle, square, triangle;

function setup() {
  circle = new draggableCircle(xPos,yPos,width,strokeColor,fillColor);
  square = new draggableRect(xPos,yPos,width,height,strokeColor,fillColor);
  triangle = new draggableTriangle(xPos,yPos,width,strokeColor,fillColor);
}

function draw() {
  background(255);
  circle.display();
  square.display();
  triangle.display();
}
```
