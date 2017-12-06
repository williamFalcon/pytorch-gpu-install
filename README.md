# create conda env
conda create -n torch python=3.6

# install numpy
pip install numpy

# install torch
conda install pytorch torchvision -c pytorch

# install cuda
conda install cuda80 -c soumith

# test gpu install
python -c 'import torch; print(torch.rand(2,3).cuda())'
