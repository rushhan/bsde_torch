# bsde_torch
A pytorch implementation of Backward Stochastic Differential Equation

# [Deep BSDE Solver](https://doi.org/10.1073/pnas.1718942115) in Torch

## To execute:
```
python main.py
```

## Currently Supports and Tested (CPU only):
* `HJBLQ`: Hamilton-Jacobi-Bellman (HJB) equation.

More to follow!!

## Dependencies
torch 1.10.0
munch 2.5.0
torchvision 1.6.3

## Reference
[1] Han, J., Jentzen, A., and E, W. Overcoming the curse of dimensionality: Solving high-dimensional partial differential equations using deep learning,
<em>Proceedings of the National Academy of Sciences</em>, 115(34), 8505-8510 (2018). [[journal]](https://doi.org/10.1073/pnas.1718942115) [[arXiv]](https://arxiv.org/abs/1707.02568) <br />
[2] E, W., Han, J., and Jentzen, A. Deep learning-based numerical methods for high-dimensional parabolic partial differential equations and backward stochastic differential equations,
<em>Communications in Mathematics and Statistics</em>, 5, 349–380 (2017). 
[[journal]](https://doi.org/10.1007/s40304-017-0117-6) [[arXiv]](https://arxiv.org/abs/1706.04702)


## Note and Thanks:
This Repo is heavily based on the work done by [[frankhan91]](https://github.com/frankhan91). THe original work is in Tensorflow and can be found [[here]](https://github.com/frankhan91/DeepBSDE). The current model reuses the same network for all the subswquent time step insteaad of creating new for each time step. This greatly reduced the parameters to train (about 1/20 the of the tf counterpart).
