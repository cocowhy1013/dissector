# dissector

Understanding behaviors of convolutional neural networks on image classification

# Requirements

- Install PyTorch ([pytorch.org](http://pytorch.org))
- *Pretrained model and dataset

# How to use

Suppose we have ImageNet dataset and pretrained ResNet101 model and corresponding pretrained 6 submodels.

1. Create several folders in `data` folder.

- `data/imagenet`: root folder of imagenet dataset

- `data/imagenet/data`: root folder of imagenet dataset files

- `data/imagenet/models/resnet101`: root folder of ResNet101 model for imagenet dataset

- `data/imagenet/tensor_pub`: root folder for anatomy outputs

- `data/imagenet/weight` root folder for weights of weight models

2. Put pretrained submodels model in `data/imagenet/models/resnet101`.

3. Create file `layer_info` to write layers' info, which the layers are used for anatomy.

    For each row, write `layer_name,layer's output size`

4. Run anatomy to produce results.

    `python anatomy.py` or `sh imagenet.sh`

Use `--help` to see arguments.

## Download example folder for imagenet dataset 