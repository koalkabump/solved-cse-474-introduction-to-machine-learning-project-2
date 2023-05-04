Download Link: https://assignmentchef.com/product/solved-cse-474-introduction-to-machine-learning-project-2
<br>



<h1>1          Task</h1>

This project is to implement neural network and convolutional neural network for the task of classification.

The classification task will be that of recognizing an image and identify it as one of ten classes. You are required to train the classifiers using Fashion-MNIST clothing images. Following are the three tasks to be performed:

<ol>

 <li>Build a Neural Network with one hidden layer to be trained and tested on Fashion-MNISTdataset. Code from scratch in Python.</li>

 <li>Build multi-layer Neural Network with open-source neural-network library, Keras on FashionMNIST dataset.</li>

 <li>Build Convolutional Neural Network (CNN) with open-source neural-network library, Keras onFashion-MNIST dataset.</li>

</ol>

Evaluate the results obtained by each of the classifier (Single layer Neural Network, Multi-Layer neural network and CNN) as shown in the evaluation section.

<h1>2          Dataset</h1>

For training and testing of our classifiers, we will use the Fashion-MNIST dataset. The Fashion-MNIST is a dataset of Zalando’s article images, consisting of a training set of 60,000 examples and a test set of 10,000 examples. Each example is a 28×28 grayscale image, associated with a label from 10 classes.

Each image is 28 pixels in height and 28 pixels in width, for a total of 784 pixels in total. Each pixel has a single pixel-value associated with it, indicating the lightness or darkness of that pixel, with higher numbers meaning darker. This pixel-value is an integer between 0 and 255. The training

Figure 1: Example of how the data looks like.

and test data sets have 785 columns. The first column consists of the class labels (see above), and represents the article of clothing. The rest of the columns contain the pixel-values of the associated image.

Each training and test example is assigned to one of the labels as shown in table 1.

<table width="126">

 <tbody>

  <tr>

   <td width="32">1</td>

   <td width="94">T-shirt/top</td>

  </tr>

  <tr>

   <td width="32">2</td>

   <td width="94">Trouser</td>

  </tr>

  <tr>

   <td width="32">3</td>

   <td width="94">Pullover</td>

  </tr>

  <tr>

   <td width="32">4</td>

   <td width="94">Dress</td>

  </tr>

  <tr>

   <td width="32">5</td>

   <td width="94">Coat</td>

  </tr>

  <tr>

   <td width="32">6</td>

   <td width="94">Sandal</td>

  </tr>

  <tr>

   <td width="32">7</td>

   <td width="94">Shirt</td>

  </tr>

  <tr>

   <td width="32">8</td>

   <td width="94">Sneaker</td>

  </tr>

  <tr>

   <td width="32">9</td>

   <td width="94">Bag</td>

  </tr>

  <tr>

   <td width="32">10</td>

   <td width="94">Ankle Boot</td>

  </tr>

 </tbody>

</table>

Table 1: Labels for Fashion-MNIST dataset

You can simply load the Fashion MNIST dataset using fashion mnist reader notebook present inside the scripts folder.

<h1>3          Plan of Work</h1>

<ol>

 <li><strong>Extract feature values and labels from the data: </strong>Fashion MNIST dataset is downloaded and processed into a Numpy array that contains the feature vectors and a Numpy array that contains the labels using fashion mnist reader notebook present inside the scripts folder.</li>

 <li><strong>Data Partitioning: </strong>The Fashion MNIST dataset is originally partitioned into a training set and a testing set. You will use this partition and train your model on the training set.</li>

 <li><strong>Train using Neural Network with One Hidden Layer </strong>Use Gradient Descent for neural network to train the model using a group of hyperparameters. (Code from scratch in python)</li>

 <li><strong>Train using Multi-Layer Neural Network </strong>with high level Neural Network library, Keras using a group of hyperparameters.</li>

 <li><strong>Train using Convolution Neural Network </strong>with high level Neural Network library, Keras using a group of hyperparameters.</li>

 <li><strong>Tune hyper-parameters: </strong>For steps 3, 4 and 5: Validate the classfication performance of your model on the validation set. Change your hyper-parameters and repeat the step. Try to find what values those hyperparameters should take so as to give better performance on the testing set.</li>

 <li><strong>Test your machine learning scheme on the testing set: </strong>For steps 3, 4 and 5: After tuning the hyper-parameters, fix your hyper-parameters and model parameter and test your models performance on the testing set. This shows the ultimate effectiveness of your models generalization power gained by learning.</li>

</ol>

<h1>4          Evaluation</h1>

<ol>

 <li>Plot graph of training loss vs number of epochs while training on each classifier (Neural Networkwith single hidden layer, multi-layer neural network and convolutional neural network).</li>

 <li>For each classifier evaluate solution on the test set using classification accuracy:</li>

</ol>

(1)

Where where <em>N<sub>correct </sub></em>is the number of corrected classified data samples, and <em>N </em>is the total number of samples of the validation set.

<ol start="3">

 <li>Construct a confusion matrix for each classifier and observe the relative strengths and weaknesses.</li>

</ol>

<h1>5          Deliverables</h1>

There are two deliverables: report and code. After finishing the project, you may be asked to demonstrate it to the TAs, particularly if your results and reasoning in your report are not clear enough.

<ol>

 <li>Report (30 points)</li>

</ol>

The report should describe your results, experimental setup and comparison between the results obtained from different setting of the algorithm. Submit the PDF on a CSE student server with the following script:

submitcse474 proj2.pdf for undergraduates submitcse574 proj2.pdf for graduates

<ol start="2">

 <li>Code (70 points)</li>

</ol>

The code for your implementation should be in Python only. You can submit multiple files, but the name of the entrance file should be main.ipynb. Please provide necessary comments in the code. Python code and data files should be packed in a ZIP file named proj2code.zip. Submit the Python code on a CSE student server with the following script:

submitcse474 proj2code.zip for undergraduates submitcse574 proj2code.zip for graduates