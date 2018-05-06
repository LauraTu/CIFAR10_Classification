# CIFAR10 classification
## 3CONV_MNIST
This is a project on CIFAR10 dataset classification using tensorflow with the 3 convolutional-block neural network architecture.

### Network Architecture
+ 3 64-hidden\_dim convolutional layers, kernel\_size = 3
+ 1 maxpooling layer
+ 3 128-hidden\_dim convolutional layers, kernel\_size = 3
+ 1 maxpooling layer
+ 3 256-hidden\_dim convolutional layers, kernel\_size = 3
+ 1 maxpooling layer
+ 1 flatten layer
+ 2 dense layers with dropout, dim\_1 = 512, dim\_2=1024
+ 1 logits layer

### Parameters
+ Input_size = [32\*32\*3], reshape to [32,32,3]
+ Batch_size = 64
+ Output_size = 10
+ Starter\_learning\_rate = 1e-2
+ Lr\_decaying\_rate = 0.96 per epoch
+ Optimizer = GradientDescentOptimizer
+ Dropout_rate = 0.2
+ Training_size = 45000
+ Validation_size = 5000
+ Testing_size = 10000

### Results
[Epoch 50]

	train_loss=0.000057, train_acc=0.908014
	valid_loss=1.018119, valid_acc=0.908545
	test_loss =1.030790, test_acc =0.908230
