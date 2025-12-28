### Q1 

	You will use CIFAR-10 Dataset (60,000 color images (32×32×3) and 10 classes (airplane, car, bird, cat, deer, dog, frog, horse, ship, truck)). You can download CIFAR-10 using:
	PyTorch: torchvision.datasets.CIFAR10
	TensorFlow: tf.keras.datasets.cifar10
	You’ll work on gray level images. Convert your image into gray level

	Design and implement a feedforward neural network for classifying the images in this dataset. You may use deep learning frameworks of your choice, e.g. PyTorch, TensorFlow. You are allowed to experiment with different number of layers/neurons, activation functions, optimizers and regularization techniques. 


#### 1. Split your dataset into training, validation and test set 

#### 2. Report loss function to evaluate your model’s performance on training and validation set. 

#### 3. Assess the model’s overall classification accuracy on the test set.  

#### 4. Prepare a report summarizing your model’s architecture, data splitting strategy, and performance of the model.  

### Q2
You will assess your model’s performance under adversarial attacks. The attacks may come through manipulated inputs, or through modifications on the algorithm. You will simulate two scenarios, and report your model’s vulnerability levels under such circumstances. 

#### a.
	There are various approaches to simulate a malicious input. You will adapt Pixel Gauss Fuzzing (PGF) [1] on the input images. This approach adds noise to the randomly selected pixels following Gaussian distribution N(μ, δ2). You may start by setting μ to be 0 and δ to be 0.8. This fuzzing technique will be applied on test images only, and the model will be used to classify these fuzzed images. Report the model’s misclassification accuracy on the fuzzed images for different parameter configurations (μ, δ).

#### b.
	As the second part, you will adapt Gauss Fuzzing [1] on model weights. This technique adds noise to the weights of a neuron following Gaussian distribution. You may initially set μ to be 0 and δ to be 0.1. You will apply this fuzzing technique on your model that is implemented in Q1, pretending that the model is manipulated by an attacker. Later, you will assess the manipulated model on original test images.  Report the models’ misclassification accuracy for different models (weights). 

#### Reference
[1] Z. Wang, H. You, J. Chen, Y. Zhang, X. Dong and W. Zhang, "Prioritizing Test Inputs for Deep Neural Networks via Mutation Analysis," 2021 IEEE/ACM 43rd International Conference on Software Engineering (ICSE), Madrid, ES, 2021, pp. 397-409, doi: 10.1109/ICSE43902.2021.00046.