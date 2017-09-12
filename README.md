# improved-gan
Initial code forked from the paper "Improved Techniques for Training GANs"

MNIST, SVHN, CIFAR10 experiments in the mnist_svhn_cifar10 folder

imagenet experiments in the imagenet folder

# goal for the ongoing work

In Semi-supervised learning scenarios the data produced by the trained GAN generator network gets used as training data for a new classifier. Consider that we can condition the latent variables on the input of the GAN on a protected parameter. Then the generated GAN output will belong to a specific subcluster inside the original real world data distribution. In this work we will focus on using these subclusters to create a metric for fairness of the target classifier and feed that into a loss function to adjust the model parameters during training.

# motivation

Neural Networks apply complex non-linear transformations to the input data. Therefore it is not straightforward to uncover hidden dependencies in the internal structure of the transformed data that might be influencing the outputs of the network. Such hidden biases embedded in the training data may lead to a NN Classifier which achieves a very high score on a hold out test set or new completely unseen test data, however it may also show unwanted discriminatory behaviours. We need better tools to allow us to audit Neural Networks and evaluate them on multiple metrics related to fairness and accountability. Relying on a single accuracy score metric is not enough in real world ML applications.   