Everything in OpenGL is in the 3D space, but the screen and the window are a 2D array of pixels
	 Because of this a large part of OpenGL is transforming the 3D coordinates to 2D pixels, which is managed by the [[graphics pipeline|Graphics Pipeline]] of OpenGL and a ton of math

To start drawing something in OpenGL, we first have give it some input vertex data
	Since OpenGL is a 3D library, we specify all coordinates in 3D($x,y,z$) 

OpenGL does not simply transform all the 3D coordinates to 2D pixels on your screen; it only processes the vertices when they are in a specific range between -1.0 and 1.0
	This range is called **normalized device coordinates**, which end up visible on your screen

The vertex shader has a few steps:
	1. Creating memory on the GPU where we store the vertex data
	2. Configuring how OpenGL should interpret the memory
	3. Specify how to send the data to the graphics card
	4. Process as much vertices as we tell it from its memory

We manage this memory via the vertex buffer object(VBO)
	This can store a large number of vertices in the GPU's memory
	This allows us to send large batches of data all at once to the graphics card(we can keep it there if there's enough memory left)
		This makes it so we do not have to send data one vertex at a time
	Once the data is in the memory of the graphics card, the shader can access the data almost instantly, which is amazing because sending data from the CPU to the GPU is relatively slow
		We always try to send as much data as possible because of this
So, OpenGL has many types of buffer objects and the buffer type of a vertex buffer is `GL_ARRAY_BUFFER`
OpenGL allows us to bind to several buffers at once as long as they have a different buffer type. 
	Use the `glBindBuffer` function to bind a target to a buffer object
		the two parameters are the target(like `GL_ARRAY_BUFFER)` and the buffer object `VBO`


After binding a buffer, any buffer calls we make will be used to configure the currently bound buffer

Then, we can make a call to the `glBufferData` function that copies the previously defined vertex data into the buffer's memory

`glBufferData` is a function specifically targeted to copy user-defined data into the currently bound buffer.
	4 parameters: target that VBO is currently bound to, size of data in bytes we want to pass to buffer, actual data, how we want the graphics card to manage the given data
		The fourth parameter has 3 forms: GL_STATIC_DRAW, GL_STREAM_DRAW, GL_DYNAMIC_DRAW
			Static draw is for position data that does not change and is used by GPU frequently, stream is for position data that does not change and the GPU uses at most a few times.  dynamic draw is for data that is used and changed frequently, by keeping the data in the memory

# Vertex Shader
 vertex shader deal with vertices
 begins with the declaration of its version
 next declare all the input vertex attributes in the vertex shader with the `in` keyword
 Vectors in GLSL have a maximum size of 4(x,y,z,w) and are incredibly useful in graphics programming because they neatly represent positions/directions in any space and has useful mathematical properties
	 vec.w represents something called the perspective division
In order to use the shader it has to dynamically compile at run-time from its source code. So, the first thing we need to do is create a shader object, referenced by an ID, stored as an unsigned int
Then, we can create the shader with `glCreateShader`, using the shader object as the argument
Next, we have to attached the shader source code to the shader object and compile the shader
	`glShaderSource` takes in 4 parameters, the shader object, how many strings we're passing as source code, the actual source code of the vertex shader, and NULL
	`glCompileShader` takes in the shader object



# Fragment Shader
Places pixels one-by-one onto the screen from the texture
Sets the fragmentColor by taking in a texture and position vector
 