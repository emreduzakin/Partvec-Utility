# Partvec-Utility

This repository contains two separate C programs:


- **part_to_perm.c**: This program converts a partition vector, represented as a list of integers, into a permutation vector.

- **perm_to_mat.c**: This program applies a permutation vector to a matrix read in Matrix Market format and outputs a new matrix with rows reordered with respect to the provided permutation vector.

## Compilation and Usage of part_to_perm.c

1. **Compilation**: Compile the code using GCC.

2. **Execution**: Run the program with the path to the partition vector file "./a.out [path-to-partvec]".

3. **Output**: The program generates a file containing the permutation vector. The output filename is created from the input filename with the last 8 characters altered to end in 'permvec'.

## Notes
- Make sure that the input file format is correct and contains one integer per line.
- This program is a work in progress and may include optimizations in the future.



## Compilation and Usage of perm_to_mat.c

1. **Compilation**: Compile the code using GCC.


2. **Execution**: Run the program by providing the path to the Matrix Market file and the permutation vector file "./a.out [path-to-matrix] [path-to-permvec]".

3. **Output**: The program generates a file containing the permutated matrix. The output filename is created from the input matrix filename with `_reordered.txt` added to the end. 

## Notes

- The input matrix must be in the Matrix Market format, and the permutation vector file should contain one integer per line.
- The program currently outputs the result in a text file, but future versions will output in Matrix Market format.
- This program is a work in progress and may include optimizations in the future.
- The program does not check wheter the provided permutation vector contains invalid or contradicting permutations.
