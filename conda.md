## Setting up environments with anaconda

### For typical eploratory data analysis

1. Create a separate envoronment callled `eda`
```
conda create -n eda python=3.6
```

2. Activate basic packages 
```
conda activate eda

conda install jupyter pandas matplotlib
```




### For OpenCV 

1. Create a separate envoronment callled `cv`
```
conda create -n cv python=3.6
```

2. Install OpenCV in the environment
```
conda activate cv
```

```
conda install opencv
```


### For TensorFlow

1. Create a separate envoronment for each TensorFlow version.

For 1.3 with python 3.5, 
```
conda create -n tf13 python=3.6
conda activate tf13
conda install -c conda-forge tensorflow==1.3
```

For 1.1, 
```
conda create -n tf11 python=3.6
conda activate tf11
conda install tensorflow
```
