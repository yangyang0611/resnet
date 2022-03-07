# Deep Residual Learning for Image Recognition: CIFAR-10, PyTorch Implementation

An implementation of the "ResNet" paper *Deep Residual Learning for Image Recogniton* [1]. This PyTorch implementation produces results within 1% of the authors' reported test error. 

The main procudure is describe as jupyter notebook in `main.ipynb` viewable [here](https://nbviewer.jupyter.org/github/a-martyn/resnet/blob/master/main.ipynb).

## Architecture
Below are the architure of different layers.

![](https://imgur.com/rzH1Clc.jpg)

## Dataset
The CIFAR-10 experiment from section 4.2 of the paper is reproduced. The goal is to classify tiny 32x32 pixel images into one of 10 classes. Some examples below. This implementation achieves 92.67% test set accuracy in this setting.

![](https://imgur.com/buOAdgll.jpg)

## Requirements
You will need the following to run the above:

- TensorFlow
- Pytorch
- Colab
If your computer didn’t have GPU, it will consume plenty of time for training

## Results from Original Paper
![](https://imgur.com/dsqPWO7l.jpg)

## Results from Implementation
![](https://imgur.com/N9A4Ffml.jpg)

## Best test error

| Architecture | #layers | % Test Error (original paper) | % Test Error (this implementation)  |
| --- | --- | --- | --- |
| Plain Net | 20 | 9.5\* | 9.5 |
| Plain Net | 32 | 10\* | 9.92 |
| Plain Net | 44 | 12\* | 11.35 |
| Plain Net | 56 | 13.5\* | 12.76 |
| ResNet | 20 | 8.75 | 8.0 |
| ResNet | 32 | 7.51 | 7.51 |
| ResNet | 44 | 7.17 | 7.38 |
| ResNet | 56 | 6.97 | 7.33 |

## References
[1] K. He, X. Zhang, S. Ren, and J. Sun. Deep residual learning for image recognition. In CVPR, 2016.

[2] C.-Y. Lee, S. Xie, P. Gallagher, Z. Zhang, and Z. Tu. Deeply-supervised nets. arXiv:1409.5185, 2014.

[3] Nitish Srivastava and Geoffrey Hinton and Alex Krizhevsky and Ilya Sutskever and Ruslan Salakhutdinov. Dropout: A Simple Way to Prevent Neural Networks from Overfitting. Journal of Machine Learning Research, 2014

[4] K. He, X. Zhang, S. Ren, and J. Sun. Identity mappings in deep residual networks. In ECCV, 2016
