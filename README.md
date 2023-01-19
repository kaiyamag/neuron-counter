# neuron-counter
A convolutional neural network to count the number of neurons in microscope images of cell tissue. Developed in a team as a course final project.

## Description:
Our neuron-counting model is based off of the [Object Classification example notebook](https://www.tensorflow.org/hub/tutorials/object_detection) from TensorFlow. We adapted the basic functions (build_dataset, build, compile, and train model, and print accuracy metric charts) to our goal of predicting the number of neurons in an image of cell tissue. A focus of this project is using transfer learning to iteratively adapt a pre-existing model to a specialized problem.

Check out [this collaborative blog post](https://medium.com/@jgb2162/neuron-counting-neural-network-c2340391d756) about our development process and an analysis of our results!

Training data: https://www.kaggle.com/datasets/jamiebergen/neurondata-th-anna1


## Usage:
The attached Jupyter Notebook contains the latest iteration of the neuron-counting model and testing benchmarks. The model can be retrained with new parameters or an expanded dataset. When adding/removing images from the dataset, ensure that `data_dir` is set to the directory of the original images, and that `neuron_labels` is an array of the integer counts associated with each image in alphanumeric order. Changing `NUM_AUGMENTATIONS` will change the number of rotated copies of each image used to supplement the dataset, and will automatically update the image labels to match the supplemented dataset.
