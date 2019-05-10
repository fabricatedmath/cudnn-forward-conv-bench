# cudnn-forward-conv-bench
Simple cudnn forward benchmark using 5x5 (from http://www.goldsborough.me/cuda/ml/cudnn/c++/2017/10/01/14-37-23-convolutions_with_cudnn/)

run with 
``` make && ./conv tensorflow.png```

I'm getting:



On a 2080TI:
```
GPU: 0
With sigmoid: false
Input Image: 578 x 549 x 3
Output Image: 584 x 555 x 3
Workspace size: 0MB
0
f() took 344 microseconds
f() took 280 milliseconds to do 1000 iterations
Wrote output to cudnn-out.png
``` 
On a Jetson Nano:
```
GPU: 0
With sigmoid: false
Input Image: 578 x 549 x 3
Output Image: 584 x 555 x 3
Workspace size: 1.85464MB
1944728
f() took 91178 microseconds
f() took 14452 milliseconds to do 1000 iterations
Wrote output to cudnn-out.png
```



