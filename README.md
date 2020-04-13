# Dog_Breed_Classifier

Identify dog breed using convolutional neural network(CNN)

Udacity Data Scientist Nanodegree Capstone Project

Check the descriptive Medium blog post [here](https://medium.com/@cloverlym/from-zero-to-one-how-i-write-my-first-deep-learning-algorithm-e0a9428192d5).

## Project Motivation

This project builds up three CNNs and an algorithm to identify the breed of dogs in images and differentiate dogs with humans as well as other objects/species.

## Installation

1.Install Anaconda if you have not installed it. Otherwise, skip this step.

2.Update Anaconda by typing conda update -all in Anaconda Prompt.

3.Clone this repository to your local machine using:

`$ git clone https://github.com/YueminLi/Dog_Breed_Classifier.git`

4.Download the following two pre-trained models and save them into a new folder named `bottleneck_features` in the Dog_Breed_Classifier repository:

[VGG16](s3-us-west-1.amazonaws.com/udacity-aind/dog-project/DogVGG16Data.npz) bottleneck features

[ResNet-50](s3-us-west-1.amazonaws.com/udacity-aind/dog-project/DogResnet50Data.npz) bottleneck features

5. Create a new folder named `saved_models` in the Dog_Breed_Classifier repository.

6.Run this Jupyter notebook in your local Anaconda Jupyter Notebook environment:

`dog_app.ipynb`

## File Descriptions

- `haarcascades`: folder contains pre-trained face detectors
  - `haarcascade_frontface_alt.xml`: the pre-trained face detector used in the `dog_app.ipynb` notebook
  
- `images`: folder contains all example images shown in the `dog_app.ipynb` notebook

- `test`: folder contains all test images used to test the algorithm in step 7

- `dog_app.ipynb`: Jupyter notebook that contains full codes to build up CNNs and algorithm

- `extract_bottleneck_features.py`: Python function to extract bottleneck features

- `bottleneck_features`: folder contains pre-trained models
  - `DogVGG16Data.npz`: pre-trained VGG16 model (this will need to be downloaded from the link provided above)
  - `DogResnet50Data.npz`: pre-trained ResNet-50 model (this will need to be downloaded from the link provided above)
  
- `saved_models`: folder contains trained models from the `dog_app.ipynb` notebook (all are saved while running the `dog_app.ipynb`)
  - `weights.best.from_scratch.hdf5`: stores the trained model with the best validation loss from self-created CNN
  - `weights.best.VGG16.hdf5`: stores the trained model with the best validation loss from VGG16 model
  - `weights.bes.Resnet50.hdf5`: stores the trained model with the best validation loss from ResNet-50 model

- LICENSE

- README.md

## Author

Yuemin Li 

Github: https://github.com/YueminLi

LinkedIn: https://www.linkedin.com/in/yuemin-li-89166333/

## License

Usage is provided under the MIT License. See LICENSE for the full details.
