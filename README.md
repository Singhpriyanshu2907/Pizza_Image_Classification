# Pizza_Image_Classification

**Data & Model Link:**  https://drive.google.com/drive/folders/1-59CyYvkZqllhnrMz3kbGy-0JJQK4MOu?usp=sharing


**Model Name:** PizzaVsNotPizzaVGG19

**Description:**

This model is designed to classify images into two categories: "pizza" and "not pizza." It employs the VGG19 architecture, a popular deep learning model known for its excellent performance in image classification tasks.

**Architecture:**

**Input Layer:** The model takes as input a 224x224x3 image, representing the RGB channels of the pizza or non-pizza image.

**Convolutional Layers:** The VGG19 architecture consists of 16 convolutional layers. Each layer applies filters to the input image, extracting features at different scales and orientations. The filters are followed by ReLU activation functions to introduce non-linearity.

**Pooling Layers:** Max pooling layers are interspersed between some of the convolutional layers. These layers downsample the feature maps, reducing computational complexity and capturing the most important features.

**Fully Connected Layers:** After the convolutional and pooling layers, the model transitions to three fully connected layers. These layers combine the extracted features into a single vector, which represents the image's features.

**Output Layer:** Finally, the fully connected layers are followed by a softmax activation function, which produces probabilities for each class. The class with the highest probability is assigned as the model's prediction.


**Training:**

**Dataset:** A large dataset of pizza and non-pizza images is required to train the model. The images should be of high quality and diverse, covering different pizza styles, angles, and lighting conditions.

**Data Preprocessing:** The images are typically resized to 224x224 pixels and normalized to have zero mean and unit variance.

**Loss Function:** The categorical cross-entropy loss function is commonly used to measure the difference between the model's predicted probabilities and the true labels.

**Optimization:** The model's weights are updated using an optimization algorithm, such as stochastic gradient descent (SGD) or Adam.

**Hyperparameters:** Various hyperparameters, including learning rate, batch size, and regularization techniques, need to be tuned to achieve optimal performance.


**Evaluation:**

**Metrics:** The model's performance is evaluated using metrics like accuracy, precision, recall, and F1-score. These metrics measure the model's ability to correctly classify pizza and non-pizza images.

**Confusion Matrix:** A confusion matrix can be used to visualize the model's performance in more detail, showing the number of correct and incorrect classifications for each class.

