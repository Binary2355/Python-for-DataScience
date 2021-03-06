# Python-for-DataScience
A record of some important point when using python such as pandas when doing data science
## Vectorization & Functional programming
* first explanation:

  Many CPUs have "vector" or "SIMD" instruction sets which apply the same operation simultaneously to two, four, or more pieces of data. Modern x86 chips have the SSE instructions, many PPC chips have the "Altivec" instructions, and even some ARM chips have a vector instruction set, called NEON.

  "Vectorization" (simplified) is the process of rewriting a loop so that instead of processing a single element of an array N times, it processes (say) 4 elements of the array simultaneously N/4 times.

* second explanation:

  Vectorization is used greatly in scientific computing where huge chunks of data needs to be processed efficiently.

  Numpy (package for scientific computing in python) , uses vectorization for speedy manipulation of n-dimensional array ,which generally is slower if done with in-built python options for handling arrays.

  although tons of explanation are out there , HERE'S WHAT VECTORIZATION IS DEFINED AS IN NUMPY DOCUMENTATION PAGE

  Vectorization describes the absence of any explicit looping, indexing, etc., in the code - these things are taking place, of course, just “behind the scenes” in optimized, pre-compiled C code. Vectorized code has many advantages, among which are:

  * vectorized code is more concise and easier to read
  * fewer lines of code generally means fewer bugs
  * the code more closely resembles standard mathematical notation (making it easier, typically, to correctly code mathematical constructs)
  * vectorization results in more “Pythonic” code. Without vectorization, our code would be littered with inefficient and difficult to read for loops.
  
  ## Pandas
  ### Essential Basic Functionality
    https://pandas.pydata.org/pandas-docs/stable/user_guide/basics.html#essential-basic-functionality
  ### Cpython extensions for pandas
  * %timeit -n 10
  * %prun -l 4
  
  This tutorial assumes you have refactored as much as possible in Python, for example by trying to remove for-loops and making use of NumPy vectorization. It’s always worth optimising in Python first.
  
  https://pandas.pydata.org/pandas-docs/stable/user_guide/enhancingperf.html#cython-writing-c-extensions-for-pandas
