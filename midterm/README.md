## Process Documentation

This is my process of experimenting with solution 1, outlined in the presentation. 

### Step 1

Create a model in Cinema 4D

### Step 2

Create a particle generator that create points on the model with XPresso

1. Bring the object into XPresso
2. Use the Particle Born node to generate particles
3. Scatter the particles' positions using Particle Surface Position node and Set Data node
4. Use the Time node and Compare node to stop the Born node from creating new particles every frame
4. Find the particles nearby one particle and connect them

### Step 3

1. Pass the points to Python
2. Create splines from the points with the Python node inside Cinema 4D's XPresso

Pseudocode:

If it’s frame 1:
- list = empty list to hold points on the model
- list.append(points to connect)
- spline = variable to hold c4d SplineObject’s linear spline
- Pass the list to SplineObject to create spline
- Insert spline into the scene under snail_geometry
- Notify Cinema 4D that the geometry has been added


### References Used

Toolfarm’s Learning Python to Expand Cinema 4D Tutorials
https://www.toolfarm.com/tutorial/c4d_spotlight_python_to_expand_cinema_4d/

The Official Cinema 4D S24.111 Python Documentation
https://developers.maxon.net/docs/Cinema4DPythonSDK/html/index.html

Cineversity’s Scripting with Python and Xpresso Tutorials
https://www.cineversity.com/learn/Scripting/
