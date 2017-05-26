 We need objloader and main files .If we try to run them as it is it will show an error
 """Traceback (most recent call last): 
  File "main.py", line 34, in <module>
    obj = OBJ('cube.obj', swapyz=False) #for any object file cube.obj
  File "/home/animesh/Documents/obj/objloader.py", line 61, in __init__
    self.mtl = MTL(values[1])
  File "/home/animesh/Documents/obj/objloader.py", line 7, in MTL
    for line in open(filename, "r"):
IOError: [Errno 2] No such file or directory: 'cube.mtl'"""
So we need cube.mtl also in the directory, the cube.mtl file is the object file's material file.
So then i copied cube.obj and cube.mtl file from https://gist.github.com/noonat/1131091
And now if I run the >>>python main.py
                     >>>It will show the openGL window

# The .obj file is an extension of 3d image I have created a method how to load and display such files.
Src Credit : https://www.pygame.org/wiki/OBJFileLoader
This code provides a function for loading a model from a wavefront OBJ file (3d model format) into an OpenGL display list. It additionally loads any referenced material and texture files. It does not support multiple models in the OBJ file, nor any material properties other than diffuse colour (Kd) and diffuse texture (map_Kd).
