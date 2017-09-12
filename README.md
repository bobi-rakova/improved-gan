# improved-gan
Initial code forked from the paper "Improved Techniques for Training GANs"

MNIST, SVHN, CIFAR10 experiments in the mnist_svhn_cifar10 folder

imagenet experiments in the imagenet folder

# goal for the ongoing work
In Semi-supervised learning scenarios the data produced by the trained GAN generator network gets used as training data for a new classifier. Consider that we can condition the latent variables on the input of the GAN on a protected parameter. Then the generated GAN output will belong to a specific subcluster inside the original real world data distribution. In this work we will focus on using these subclusters to create a metric for fairness of the target classifier and feed that into a loss function to adjust the model parameters during training.

