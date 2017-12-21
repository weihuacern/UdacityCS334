# UdacityCS334

Enable nvcc command to compile cuda and OpenCV:
```
source EnvSet.sh
```
The Information contained in the EnvSet.sh:
```
export PATH=/usr/local/cuda-9.0/bin${PATH:+:${PATH}}
or
export PATH=$PATH:/usr/local/cuda-8.0/bin
export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/usr/local/lib
```
Use CUDA 8.0 to be compatiable with OpenCV, 2017 Nov.

# Lesson 1 The GPU Programming Model
```
nvcc -o cube cube.cu
```

# Lesson 2 GPU Hardware and Parallel Communication Patterns
```
nvcc -o hello_threadIdx hello_threadIdx.cu
nvcc -o hello_blockIdx hello_blockIdx.cu
nvcc -o associative associative.cu
nvcc -o memory memory.cu
nvcc -o atomics atomics.cu
```

# Lesson 3 Fundamental GPU Algorithms (Reduce, Scan, Histogram)

Compare the global and shared memory in reduce, 0 for global, 1 for shared. In theory, the shared one will be 3 times faster than global version. But we cannot reach that because of the computation is not saturated. 
```
nvcc -o reduce reduce.cu
./reduce 0
./reduce 1
```
