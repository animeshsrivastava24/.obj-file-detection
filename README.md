# The .obj file is an extension of 3d image I have created a method how to load and display such files.
Src Credit : https://www.pygame.org/wiki/OBJFileLoader
This code provides a function for loading a model from a wavefront OBJ file (3d model format) into an OpenGL display list. It additionally loads any referenced material and texture files. It does not support multiple models in the OBJ file, nor any material properties other than diffuse colour (Kd) and diffuse texture (map_Kd).
