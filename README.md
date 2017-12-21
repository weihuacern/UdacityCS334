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

# Lesson 1
```
nvcc -o cube cube.cu
```

# Lesson 2
```
nvcc -o hello_threadIdx hello_threadIdx.cu
nvcc -o hello_blockIdx hello_blockIdx.cu
nvcc -o associative associative.cu
nvcc -o memory memory.cu
nvcc -o atomics atomics.cu
```
