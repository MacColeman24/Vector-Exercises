# Vector Exercises

This is a repository for testing a basic vector class. We added extra methods to the Vector2D class in order to make the CatsCradle class work properly.

Additionally, I changed some parts of the CatsCradle class to make the program more visually interesting.
The cat's cradle now has an odd number of sides, so that the edges do not converge in the center.

The way that edges are processed was also changed. Edges now are split into many smaller lines through the `splitLineIntoSegments` method I added. Each of these smaller line segments can be individually colored. I used this functionality to make the lines brightest in the middle, and darkest around the nodes of the graph. The function that controls this brightness is the `mapColor` method in CatsCradlePanel.java.

I added another instance variable to be the hue of the drawing. Hue is an HSV (HSB in java) value that steps by one degree every frame. The HSV value is then turned into an RGB value that can be used to draw the diagram. This leads to a pleasant effect where the drawing changes colors as it animates.

![The Cat's Cradle Program](/images/Example.png)

### Instructions

To display the window, simply run the CatsCradle.java class.
