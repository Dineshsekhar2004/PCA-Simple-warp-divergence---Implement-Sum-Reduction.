# PCA-Simple-warp-divergence---Implement-Sum-Reduction.
Refer to the kernel reduceUnrolling8 and implement the kernel reduceUnrolling16, in which each thread handles 16 data blocks. Compare kernel performance with reduceUnrolling8 and use the proper metrics and events with nvprof to explain any difference in performance.

## Aim:
PCA-Simple-warp-divergence---Implement-Sum-Reduction. Refer to the kernel reduceUnrolling8 and implement the kernel reduceUnrolling16, in which each thread handles 16 data blocks. Compare kernel performance with reduceUnrolling8 and use the proper metrics and events with nvprof to explain any difference in performance.
## Procedure:
Step 1 : Include the required files and library.

Step 2 : Introduce a function named 'recursiveReduce' to implement Interleaved Pair Approach and function 'reduceInterleaved' to implement Interleaved Pair with less divergence.

Step 3 : Introduce a function named 'reduceNeighbored' to implement Neighbored Pair with divergence and function 'reduceNeighboredLess' to implement Neighbored Pair with less divergence.

Step 4 : Introduce optimizations such as unrolling to reduce divergence.

Step 5 : Declare three global function named 'reduceUnrolling2' , 'reduceUnrolling4' , 'reduceUnrolling8' , 'reduceUnrolling16' and then set the thread ID , convert global data pointer to the local pointer of the block , perform in-place reduction in global memory ,finally write the result of the block to global memory in all the three function respectively.

Step 6 : Declare functions to unroll the warp. Declare a global function named 'reduceUnrollWarps8' and then set the thread ID , convert global data pointer to the local pointer of the block , perform in-place reduction in global memory , unroll the warp ,finally write the result of the block to global memory infunction .

Step 7 : Declare Main method/function . In the Main method , set up the device and initialise the size and block size. Allocate the host memory and device memory and then call the kernals decalred in the function.

Step 8 : Atlast , free the host and device memory then reset the device and check for results.


## Output:

## Result:
