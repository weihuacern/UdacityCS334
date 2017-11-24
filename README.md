# UdacityCS334

Enable nvcc command to compile cuda:
export PATH=/usr/local/cuda-9.0/bin${PATH:+:${PATH}}
export PATH=$PATH:/usr/local/cuda-8.0/bin
Compile cuda:
nvcc -o cube cube.cu
