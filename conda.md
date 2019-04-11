# Setting up environments with anaconda

## For typical eploratory data analysis

1. Create a separate envoronment callled `eda`
```
conda create -n eda python=3.6
```

2. Activate basic packages 
```
conda activate eda

conda install jupyter pandas matplotlib
```


## Install PyTorch using conda

1. Make a virtual environment
```
conda create -n torch python=3.5
```

To activate this environment, 
```
conda activate torch
```

To deactivate, 
```
conda deactivate
````

2. Install PyTorch

First, activate the environment,
```
conda activate torch
```

Install PyTorch using conda without GPU,
```
conda install pytorch torchvision -c pytorch
```

See [here](https://pytorch.org/get-started/locally/) for other options.


## Install OpenCV 

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


## Install TensorFlow

For 1.3 with python 3.5, 
```
conda create -n tf13 python=3.6
conda activate tf13
conda install -c conda-forge tensorflow==1.3
```

For 1.1 with python 3.6 (OSX), 
```
conda create -n tf11 python=3.6
conda activate tf11
conda install tensorflow
```
