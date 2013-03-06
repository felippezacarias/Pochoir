* This is the codebase for the Pochoir stencil compiler.  The codebase 
  currently is still in development.  For more information, please see:
  http://groups.csail.mit.edu/sct/wiki/index.php?title=The_Pochoir_Project

* In order to setup the Pochoir compiler, the following packages needs to be
  installed on your system:
- A Cilk Plus compiler (whether that's Intel C/C++ compiler or the open source
  gcc version).
  For more information on obtaining a compiler for Cilk Plus, see:
  http://www.cilkplus.org/which-license#gcc-development
- C++ Boost library 
- The Haskell Platform:
  http://www.haskell.org/platform/

  (mainly for 'ghc' --- the Glasgow Haskell Compiler: http://www.haskell.org/ghc/)

* Once the system prerequisites are satisfied, go into the top-level 
  directory of the Pochoir compiler (either the Pochoir_v0.5, Release_v0.5,
  of ExecSpec_v2.0) and type 'make' to build the Pochoir compiler.

* Assuming make is successful, you should see a binary in the top-level
  directory: pochoir.  For ExecSpec_v2.0, you should also find a second
  binary, genstencil, in the top-level directory.

* To run an example, go into the example directory, and make sure you 
  a. Set up the environtment variable required for pochoir:
     POCHOIR_LIB_PATH=<top-level dir for the Pochoir compiler>
  b. Copy the binaries in the top-level directory (i.e., pochoir and 
     genstencil) into your example directory.  
  c. Run make <example>, where <example> can be any file in the example
     directory without the tb_ prefix.
 