## Process Documentation

This is my process of creating the sculpture in Cinema 4D. 

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

### Step 4

1. Combine the splines
2. Use Sweep to create renderable 3D geometry

### Step 5

1. Create an object
2. Put the object in a cloner
3. Use Python to create a custom mograph effector for the cloner

### Step 6

1. Using full control to handle all clones at once, create an oscillating effect with the Python effector
2. Let the animation run until the design looks right

### Step 7

1. Combine the snail and the shell to create the model.
2. Render the image.

### References Used
[Toolfarm’s Learning Python to Expand Cinema 4D Tutorials]
(https://www.toolfarm.com/tutorial/c4d_spotlight_python_to_expand_cinema_4d/)
[The Official Cinema 4D S24.111 Python Documentation] 
(https://developers.maxon.net/docs/Cinema4DPythonSDK/html/index.html)
[Cineversity’s Scripting with Python and Xpresso Tutorials]
(https://www.cineversity.com/learn/Scripting/)
https://www.cineversity.com/vidplaytut/nab_2015_rewind_colin_sebestyen

