# vim ~/.bashrc
- add the following shortcut keys for personal use
- alias ll='ls -alF'
- alias la='ls -A'
- alias l='ls -CF'

# Anaconda
- download https://www.anaconda.com/distribution/
- cd ~/download
- wget xxxxx.sh
- chmod 777 xxxxx.sh
- ./xxxx.sh


# PyTorch
- download the version https://pytorch.org/
    - python3.6, singularity, tmux-2.9a, anaconda3-2019.10, swig-4.0.0.7, git-2.23.7, go-1.13.4.7, direnv-2.20.0.7, 
    - gcc-4.9.2, gcc-5.5.0, gcc-6.3.0, cuda-10.1.105_418.39, cuda-10.2.89_440.33.01, cudnn-10.1-linux-x64-v7.6.5.32, cudnn-10.2-linux-x64-v7.6.5.32
- tba


# >>> conda initialize >>>
# !! Contents within this block are managed by 'conda init' !!
__conda_setup="$('/home/shuk/anaconda3/bin/conda' 'shell.bash' 'hook' 2> /dev/null)"
if [ $? -eq 0 ]; then
    eval "$__conda_setup"
else
    if [ -f "/home/shuk/anaconda3/etc/profile.d/conda.sh" ]; then
        . "/home/shuk/anaconda3/etc/profile.d/conda.sh"
    else
        export PATH="/home/shuk/anaconda3/bin:$PATH"
    fi
fi
unset __conda_setup
# <<< conda initialize <<<




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


## Uninstall Pytorch

Uninstall pytorch, cmd ```conda uninstall pytorch torchvision```, if installing it using                
```conda install pytorch torchvision cuda80 -c pytorch```



Shu Kong @ CMU
March 2020
