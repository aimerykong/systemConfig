# vim ~/.bashrc
- # some more ls aliases
- alias ll='ls -alF'
- alias la='ls -A'
- alias l='ls -CF'



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
