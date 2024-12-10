# Off-by-One Error in C++ Vector Iteration

This repository demonstrates a common off-by-one error in C++ when iterating over a `std::vector`. The error occurs when the loop condition incorrectly uses `<=` instead of `<` when comparing the loop counter to the vector's size. This results in accessing an element beyond the vector's valid range, leading to undefined behavior and often a segmentation fault.

## Bug

The file `bug.cpp` contains the buggy code.  The loop iterates one element past the end of the vector causing a crash.