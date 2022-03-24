# Differentially Private CIFAR10

Image classification on CIFAR10 dataset using differential privacy.

## Experimental Setup
The system environment that will be used to assess this project consists of Apple M1/M1 pro GPU ([Metal GPUFamily Apple 7](https://developer.apple.com/documentation/metal/)) running on macOS operating system, [TensorFlow Privacy](https://www.tensorflow.org/responsible_ai/privacy/guide) as the deep learning framework coded on Python3 programming language.


## Evaluation Metric
We will be computing the training loss to assess the model. Further, to measure our model’s privacy performance, two metrics i.e., Epsilon (ϵ) and Delta (δ) will be used which are based on [Mironov’s Rényi Differential Privacy](https://arxiv.org/abs/1702.07476). The allowed privacy budget for this project is as follows: Epsilon: ϵ≤5.0; with Delta fixed to: δ=〖10〗^(-5).

To compute the value of ϵ, we will be using TensorFlow’s ["compute_dp_sgd_privacy"](https://www.tensorflow.org/responsible_ai/privacy/tutorials/classification_privacy) method which takes δ, batch size, noise multiplier, number of epochs and total number of points in training data as the input arguments.


## Team Members
1.	Sanika Katekar; sk56865@uga.edu
2.	Soham Sajekar; ss92078@uga.edu
