# NemoLib-C-V2-Testing
This program is for testing NemoLib C++ version 2, available at https://github.com/ZachBrader/NemoLib-C-V2-StaticLib. 

If you are interested in the original version, the library is available from https://github.com/Kimw6/NemoLibC, and the testing file is at https://github.com/Kimw6/NemoLibC-Testing.

The latest Java version is available at https://github.com/Kimw6/NemoLib-Java-V2.

# Installation in Linux
* download main.cpp program to the linux folder
* compile
g++ -std=c++11 -c main.cpp -o main.o -I.
* Link (for example, your NemoLib-C-V2-StaticLib.o is in the home/lib/NemoLib-C-V2-StaticLib folder)
g++ -o main main.o -Lhome/lib/NemoLib-C-V2-StaticLib -lnemolib-c-v2-staticlib
* download the "exampleGraph.txt" file.
* Run
./main

# Installation in Windows

In Netbeans with C/C++ Plugins:
* Download Files
* Open Netbeans and Select, "Open Existing Project"
* After opening the project, make sure that NemoLib-C-V2-StaticLib is set up correctly, and is built.
* Right click on this project in the projects window and select "Properties".
* Select "C++ Compiler". Under this catagory, select "Include Directories" and choose to include the NemoLib-C-V2-StaticLib files. Also make sure that the C++ version is set to C++14.
* Select "Linker".Click “Libraries”->“Add Library File” and choose the NemoLib-C-V2-StaticLib/dist/Debug/CLang-Windows/libnemolib-c-v2-staticlib.a”
* Make sure that "exampleGraph.txt" files exists in the same folder as "main.cpp". 
* Try building and running the program.
* To test other files, try modifying the command arguments.

In Visual Studios:  
* Create a new C++ project. 
* Copy "main.cpp" into the same folder as all of the files from NemoLib-C-V2-StaticLib.
* Include all the files into the project.
* Set the project's settings to C++14, Release, and x64. (The later two are for speed improvements).
* Build and run.
