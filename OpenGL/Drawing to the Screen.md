Everything in OpenGL is in the 3D space, but the screen and the window are a 2D array of pixels
	 Because of this a large part of OpenGL is transforming the 3D coordinates to 2D pixels, which is managed by the [[graphics pipeline|Graphics Pipeline]] of OpenGL and a ton of math

To start drawing something in OpenGL, we first have give it some input vertex data
	Since OpenGL is a 3D library, we specify all coordinates in 3D($x,y,z$) 

OpenGL does not simply transform all the 3D coordinates to 2D pixels on your screen; it only processes the vertices when they are in a specific range between -1.0 and 1.0
	This range is called **normalized device coordinates**, which end up visible on your screen

