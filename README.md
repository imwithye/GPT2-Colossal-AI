# CS5260, Assignment 6, Train ResNet on CIFAR-10 from scratch

[GitHub](https://github.com/imwithye/ResNet-Colossal-AI)

## 🚀 Quick Start

This example provides a training script and an evaluation script. The training script provides an example of training ResNet on CIFAR10 dataset from scratch.

- Training Arguments
  - `-p`, `--plugin`: Plugin to use. Choices: `torch_ddp`, `torch_ddp_fp16`, `low_level_zero`. Defaults to `torch_ddp`.
  - `-r`, `--resume`: Resume from checkpoint file path. Defaults to `-1`, which means not resuming.
  - `-c`, `--checkpoint`: The folder to save checkpoints. Defaults to `./checkpoint`.
  - `-i`, `--interval`: Epoch interval to save checkpoints. Defaults to `5`. If set to `0`, no checkpoint will be saved.
  - `--target_acc`: Target accuracy. Raise exception if not reached. Defaults to `None`.

- Eval Arguments
  - `-e`, `--epoch`: select the epoch to evaluate
  - `-c`, `--checkpoint`: the folder where checkpoints are found

### Demo Notebook

In the demo notebook `makeenv.ipynb`, it shows how to install and run on Google Colab.
Note that the runtime may restart multiple times for installing the dependencies.

### Some Info

The model used in the experiment:        ResNet
The dataset employed:                    CIFAR-10
Parallel settings:                       Only 1 GPU is used
Instructions on how to run your code:    In `makeenv.ipynb`
Experiment results, presented in a table or figure:

Accuracy of the model on the test images: 70.33 %

The original code runs with 80 epoches, but to reduce the time on Google Colab, only 10 epoches are ran.
So the accuracy is 70.33%.

