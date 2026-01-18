Before making a graphics, we have to do two things:
	Create a window context
	Create the application window

Instead of needing to go down to an operating system level, we use external libraries like GLFW to deal with all the OS stuff

Glad handles all of the drivers

```
int main()
{
    glfwInit();
    glfwWindowHint(GLFW_CONTEXT_VERSION_MAJOR, 3);
    glfwWindowHint(GLFW_CONTEXT_VERSION_MINOR, 3);
    glfwWindowHint(GLFW_OPENGL_PROFILE, GLFW_OPENGL_CORE_PROFILE);
    //glfwWindowHint(GLFW_OPENGL_FORWARD_COMPAT, GL_TRUE);
  
    return 0;
}
```

This code first initializes GLFW, then after configures it using Hints

```
GLFWwindow* window = glfwCreateWindow(800, 600, "LearnOpenGL", NULL, NULL);
if (window == NULL)
{
    std::cout << "Failed to create GLFW window" << std::endl;
    glfwTerminate();
    return -1;
}
glfwMakeContextCurrent(window);
```

This code first creates the window in the first line and creates a variable to hold the window. The `glfwCreateWindow` has 4 parameters, width and height, then name. The last are not important now.

Then, we check if the window variable works or not using NULL equivalence checking. 

```
if (!gladLoadGLLoader((GLADloadproc)glfwGetProcAddress))
{
    std::cout << "Failed to initialize GLAD" << std::endl;
    return -1;
} 
```

We want to initialize glad before any function in OpenGL because glad manages the function points for OpenGL

Before we start rendering anything with OpenGL, we have to tell OpenGL the size of the rendering window so OpenGL knows how we want to display data and coordinates with respect to the window

```
glViewport(0, 0, 800, 600);
```

The first two parameters set the lower left corner of the window. Then, the next two set the width and height

```
void framebuffer_size_callback(GLFWwindow* window, int width, int height);  
```

This lets the viewport be adjusted when the window is adjusted

```
glfwSetFramebufferSizeCallback(window,framebuffer_size_callback);  
```

This tells GLFW what to do

Since we want the window to stay open and not close immediately, we should run the following command

```

while(!glfwWindowShouldClose(window))
{
    glfwSwapBuffers(window);
    glfwPollEvents();    
}
```

This creates the **render loop** that keeps the program running until we get an input to close the window, which will tell GLFW to stop. 

The while loop checks that the function is returning False for any input that is telling the window to close. `glfwPollEvents` is checking for the inputs. `glfwSwapBuffers` will swap the color buffer that is used to render and show the output on the screen

```
glfwTerminate();
return 0;
```
To clean up and delete all of GLFW's resources that we allocated, we use the `glfwTerminate` function at the end of the main function, cleaning up all resources and properly exit the application

To process any input, we should make a separate function and use the built-in `glfwGetKey` function that takes the window and key as arguments

```
void processInput(GLFWwindow *window)
{
    if(glfwGetKey(window, GLFW_KEY_ESCAPE) == GLFW_PRESS)
        glfwSetWindowShouldClose(window, true);
}
```
This should be added to the *render loop*

```
glClearColor(0.2f, 0.3f, 0.3f, 1.0f);
glClear(GL_COLOR_BUFFER_BIT);
```

Using `glClearColor`, we specify the color to clear the screen. Then, we clear the color buffer using `glClear`. After this, the entire color buffer will be filled with the color that was the argument in `glClearColor`

This means `glClearColor` is a *state-setting* function and `glClear` is a *state-using* function because one specifies the state, while the other retrieves it

# Definitions
A **Frame** is single, complete image or snapshot of a scene

A **Buffer** are temporary memory areas to store image data, prevent screen tearing, and enables complex rendering by drawing them off-screen

**Rendering** is transforming code to visual

**Double Buffer**
	When using a single buffer to render, the resulting image will have flickering because images or frames are not drawn instantaneously, but rather in a sequence pixel after pixel from the top left to the bottom right
	To fix this issue, we can pre-draw two buffers instead of just one
	The *front buffer* contains the final output image, while the *back buffer* draw all the rendering commands
	Once all the commands are done, we move the back buffer to the front buffer`


