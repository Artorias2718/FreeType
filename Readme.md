# FreeType (From [LearnOpenGL.com](https://learnopengl.com/In-Practice/Text-Rendering))
## -- VS Community 2019

Getting the sample code to work might be a bit annoying, so here's what I did (if you want to do this all yourself, if not just cloning this project down should suffice):

* I downloaded all of the necessary libraries and resource files (located in Includes directory):
  * Freetype
  * GLAD (this was a bit weird initially but not too bad, just don't skip any files (I forgot the **khrplatform.h** file initially).
  * GLM
  * LearnOpenGL

* Next, you'll need to actually build **FreeType**
  * It should work for you right out of the box, just find the **VS2010** folder, open up the solution and build it.
  * Then, copy the **freetype.lib** file to **External/GLFW/Lib**
  * Copy the **freetype.dll** file to your output folder (**Debug** or **Release**)
  * Make sure you add **freetype.lib** as a dependency: **Linker => Input => Additional Dependencies**
  * Finally, don't forget about **Includes: VC++ Directories => Inlclude Directories: Set it as Includes;Resources;**. This will allow you to access the library header files as well as the Font file.
~
~

