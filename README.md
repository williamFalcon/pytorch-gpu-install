# Pytorch GPU install instructions    
At the end of these instructions you will have:   
1. A fully working conda environment running pytorch on GPUs

```bash
# create conda env
conda create -n torch python=3.6

# install numpy
pip install numpy

# install torch
conda install pytorch torchvision -c pytorch

# install cuda (8. Cuda 9 not yet supported ny pytorch)    
conda install cuda80 -c soumith

# test gpu install
python -c 'import torch; print(torch.rand(2,3).cuda())'
```
