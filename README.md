# Web assembly
Discovery project of c++ on web assembly. The goal being to reproduce known solutions on different technologies.  

## Goal
The things i'm interested in poking around in web assembly are portability and interaction of different languages.   
I'd like to see how deploying in containers with different hosts works and i'd like to see modules made in different languages can work. My idea right now would be to create an app supporting image manipulation and 3D mesh operations. Hopefully, parts in C++, parts in rust (want to play with as well) deployed on containers running windows, linus or ios. Finding a reason to play with databases would be a bonus.

# Compiler 
I've worked mostly with MSVC as a compiler, LLVM ([Emscripten](https://emscripten.org/index.html)) is the go to toolchain to compile to webassembly for c++, thus i will be switching to discover it.  
Being on windows, i've also wanted to play around developping on linux, thus **WSL** will be my new home for now.
I'm excited to have the chance to play with linux only c++ tools such as **valgrind** but hopefully not too many memory problems arise.  

# Technologies
## Frontend
I've mostly played with [**Qt (QML)**](https://doc.qt.io/qt-6/qtqml-index.html) to create GUIs. I'm excited to see what webassembly libraries exist for this.

## Meshing
I've mostly used [**VTK**](https://vtk.org/) and a little [**IGL**](https://libigl.github.io/) to have fun with mesh. Let's see what webassembly libraries are offered.

## Image manipulation
[**OpenCV**](https://docs.opencv.org/3.4/df/d0a/tutorial_js_intro.html) i've used but [**VTK**](https://vtk.org/) a lot more. **OpenCV** seems to already support webassembly to some extent. TBD

## Containers
I've only briefly explored [**Docker**](https://docs.docker.com/get-started/overview/) containers, i'd like to expand on this. I doubt [**Kubernetes**](https://kubernetes.io/) is worth it at the time of writing.

# Disclaimer
This is <ins>not meant to be production worthy</ins> in any shape or form. It is mostly meant as a technologies playground or a Proo of concept type of project. 