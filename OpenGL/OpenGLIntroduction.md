OpenGL is often maintained by the graphics card manufacturers, separately by the each OS and manufacturer

After version 3.2, OpenGL is no longer in the immediate profile and is currently using the core profile. The immediate profile does not allow developers to modify the actual calculations OpenGL does, whereas core does with increased difficulty

OpenGL by itself is a very large state machine, a collection of object, variables that define how OpenGL should currently operate
	We often change the state of OpenGL when drawing shapes, shaders, or manipulating what OpenGL is supposed to render

OpenGL libraries are written in C and allows for many derivations in multiple languages with many different abstractions like objects

An object in OpenGL is a collection of options that represents the subset of OpenGL's state
	You can visualize an object as a C-like struct:
		```struct objectName {
		float option1;
		float option2;
		char[] name;
		};
		```

