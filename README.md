📊 Coordinate System Line Plotter

This script uses specialized graphics functions (Line, add, setPosition, etc.) to draw a simple Cartesian (X-Y) coordinate grid and plot a diagonal line.

It serves as a fundamental example of working with coordinate geometry and manipulating line properties in a graphics environment.

📐 Program Functions

The program consists of three main drawing functions, all called by main():

drawXAxis(): Draws a thick horizontal line (the X-axis) across the middle of the canvas at the Y-coordinate 200.

new Line(0, 200, 400, 200); // From (0, 200) to (400, 200)


drawYAxis(): Draws a thick vertical line (the Y-axis) down the middle of the canvas at the X-coordinate 200.

new Line(200, 0, 200, 400); // From (200, 0) to (200, 400)


drawDiagonal(): Plots a thin, teal diagonal line. Although it is initialized with one set of coordinates, the subsequent calls determine the final position:

The starting point is set to (0, 50) using setPosition().

The ending point is set to (400, 250) using setEndpoint().

📌 Note on Line Coordinates

In this environment, the Line() constructor requires four arguments in this order:

$$\text{Line}(\text{Start X, Start Y, End X, End Y})$$

The functions setPosition() and setEndpoint() are then used to adjust these start and end points after the line object is created.

⚠️ Execution Warning

This code uses specific non-standard graphics objects (Line, add, setPosition, etc.). To run this file, you must execute it within the specialized environment it was written for. It will not run directly in a standard web browser without significant modification to use the HTML Canvas API.
