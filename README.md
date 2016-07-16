
Description:
============

Eye of Sauron aims to pierce all topological analyses looked accross critical
points to the interbasin surfaces.
It is a molecular visualizer that tries to satisfy the special needs of QTAIM/IQA 
and other emergent scalar fields topology analyses.
Special focus is paid to in-home programs: Critic2 and Promolden.


Requirements:
============

* Cmake and CCmake.
* Boost > 1.49.
* Manually compiled VTK-7.0.0.
  1. Download it. Extract and go into the directory.
  2. Create a build directory and run `ccmake ..` from it.
     Try to compile with OpenGL2 renderer because the
     speed is improved over OpenGL v1.
  3. Keep track of the build path for later use.

* Manually compiled openbabel.
  1. Download openbabel 2.3.2.
  2. Copy `*format.cpp` to `openbabel-*/src/formats/`. 
  3. Add the names of the files to `openbabel-*/src/formats/CMakeLists.txt`.
  4. Compile and install (cmake [install dir] ; make; install)

Installation:
==============

There is a `compile.sh` script already designed for the compiling process.
The `script.py` shows how to access the library from python.

License:
========

EyeOfSauron is distributed under the GPLv3 License.
See [Copyright.txt][] for details.

[Copyright.txt]: LICENSE.txt
