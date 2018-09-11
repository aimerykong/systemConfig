# setup pytorch and so on


## Anaconda

```cd ~/Downloads```

```wget https://repo.anaconda.com/archive/Anaconda3-5.2.0-Linux-x86_64.sh```

```bash Anaconda3-5.2.0-Linux-x86_64.sh```


## Pytorch

```conda install pytorch torchvision cuda80 -c pytorch```

### Install basic dependencies

```export CMAKE_PREFIX_PATH="$(dirname $(which conda))/../" # [anaconda root directory]```

```conda install numpy pyyaml mkl mkl-include setuptools cmake cffi typing```

```conda install -c mingfeima mkldnn```


### Add LAPACK support for the GPU

```conda install -c pytorch magma-cuda80 # or magma-cuda90 if CUDA 9```


