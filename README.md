# DoxygenCmake
Use Doxygen by Cmake Sample.

## How to generate Doxygen html files?

### Edit CMakeLists.txt
You can make doxygen html docment for any target by simple cmake function.  

Example.  
see /CMakeLists.txt:  
```
include(Doxygen/doxygen.cmake)
```
and see /Main/CMakeLists.txt:
```
add_doxygen(Main)
```

### Do Cmake Command
For out-surce-build, you follow below.
```
mkdir build
cmake ..
```

### Generate Doxygen Files.
Now you can generate doxygen html files for make target.

You can generate all target documents by `make doxygen`.
```
make doxygen
```

You can also generate single target document by `make doxygen-XXXX`.

```
make doxygen-Main
```

