---
layout: article
title: 🦋Winged Wonders
abstract: A Deep Learning Approach to Butterfly Species            Identification 🌿
categories: MachineLearning
tags: TensorFlow MobileNetV3Large ImageClassifier
eyeCatcher: https://img.rawpixel.com/s3fs-private/rawpixel_images/website_content/v430-adj-42-acrylictexture_2.jpg?w=800&dpr=1&fit=default&crop=default&q=65&vib=3&con=3&usm=15&bg=F4F4F3&ixlib=js-2.2.1&s=e283f157f1a5c95c4873022041295af0
---

---

**A Deep Learning Approach to Butterfly Species Identification 🌿**
=====================================================



<div style="text-align: left;">

  <a href='https://github.com/PhuongFX/ButterFlySpace/blob/main/LICENSE'><img style='display: inline-block; margin: 0; padding: 0;' src='https://img.shields.io/badge/License-AGPL%203.0-blue.svg' alt='License: AGPL-3.0'></a>
  <a href='https://www.python.org/'><img style='display: inline-block; margin: 0; padding: 0;' src='https://img.shields.io/badge/Python-3.x-blue' alt='Python'></a>
  <a href='https://www.tensorflow.org/'><img style='display: inline-block; margin: 0; padding: 0;' src='https://img.shields.io/badge/TensorFlow-2.x-orange' alt='TensorFlow'></a>
  <a href='https://keras.io/'><img style='display: inline-block; margin: 0; padding: 0;' src='https://img.shields.io/badge/Keras-2.x-green' alt='Keras'></a>
  <a href='https://opencv.org/'><img style='display: inline-block; margin: 0; padding: 0;' src='https://img.shields.io/badge/OpenCV-4.x-red' alt='OpenCV'></a>
  <a href='https://github.com/PhuongFX/ButterFlySpace'><img style='display: inline-block; margin: 0; padding: 0;' src='https://img.shields.io/badge/Open%20Source-%E2%9D%A4-green.svg' alt='Open Source'></a>
  <a href='https://www.kaggle.com/datasets/gpiosenka/butterfly-images40-species'><img style='display: inline-block; margin: 0; padding: 0;' src='https://img.shields.io/badge/Dataset-📊-red.svg' alt='Dataset'></a>
  
</div>
        
> Are you fascinated by the beautiful world of butterflies? 🦋 With over 20,000 known species, these delicate creatures have long been a subject of interest for entomologists and naturalists alike. However, accurate identification of butterfly species remains a significant challenge, hindering our understanding of their behavior, habitat, and conservation. 🌿

## `About`
This project is all about using deep learning to classify images of butterflies into their respective species. The dataset is from Kaggle, which contains over 10,000 images of butterflies from 100 different species. 📸
The images were collected from various sources, including field observations, museum collections, and online repositories.


## `Dataset` 📊

* **Dataset URL:** [🐛 Butterfly & Moths Image Classification 100 species](https://www.kaggle.com/datasets/gpiosenka/butterfly-images40-species)
* **License:** CC0-1.0
* **Number of images:** 12594
* **Number of classes:** 100

| Category | Number of Images |
| --- | --- |
| Training | 12594 |
| Validation | 500 |
| Testing | 500 |

## `Inspiration` 🌪️

* Manual identification of butterfly species is a time-consuming and expertise-dependent process, prone to errors and inconsistencies. 📝
* The lack of an efficient and accurate identification system hinders the study of butterfly populations, habitats, and behavior, ultimately affecting conservation efforts. 🌎
* An automated system for butterfly species identification can have a profound impact on our understanding of these insects and their role in ecosystems. 🌟


===========================================================================

## `Methodology` 🔍

> ### Requirements

* Python 3.x
* TensorFlow 2.x
* Keras
* OpenCV
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Plotly
  
> ### Data Preprocessing 🔀

* Data augmentation: Apply random transformations to the images to artificially increase the size of the training set using TF-keras pre-processing layers. 🔀
* Image resizing: Resize images to a uniform size of 224x224 pixels.

> ### Model Architecture 📚

* Base model: MobileNetV3Large model pre-trained on ImageNet (224, 224, 3)
* Custom classification head: Add a new classification head on top of the base model, consisting of global average pooling layers, batch normalization layers, and dense layers with 100 units.

> ### Training 📊

* **Optimizer:** Adam
* **Loss function:** Sparse categorical crossentropy
* **Batch size:** 32
* **Number of epochs:** 50
* **Metrics:** Accuracy

> ### Model Performance 📊

The model achieves a test accuracy of 0.96, which is a great result considering the complexity of the dataset! 🎉 Here's a breakdown of the results:

* Training accuracy: 0.9996
* Validation accuracy: 0.9420
* Test accuracy: 0.9600

> ### Future Work 🚀

* Experiment with different model architectures (ResNet or DenseNet 🤖) and hyperparameters (transfer learning to fine-tune the model on a different dataset 📚) to improve performance.

===========================================================================

## `Acknowledgments` 🙏

* Kaggle dataset: 🐛 Butterfly & Moths Image Classification 100 species
* TensorFlow and Keras libraries for deep learning
* Matplotlib and Seaborn libraries for data visualization

## `🙅‍♂️Disclaimer`

> This project is licensed under AGPL-3.0 License and is for personal use only and should not be used for commercial purposes.
The pre-trained model and may not always produce accurate results.

## `Get Involved!` 😌
This project demonstrates the potential of deep learning for butterfly species identification. 
The model achieves high accuracy and can be used as a starting point for further research and development in this field. 

I hope you found this project informative and engaging! 😊  
If you're interested in collaborating and contributing to the project, please let me know! I'd love to hear from you.
* [Follow me on GitHub](https://github.com/PhuongFX)
* [Follow me on Hugging Face](https://huggingface.co/PhuongFX)

## `Getting Started` 🚀

To get started with this project, you'll need to:

* Install the required libraries, including TensorFlow, Keras, and OpenCV 📦
* Download the dataset from Kaggle 📈
* Run the code to train and evaluate the model 🤖

Enjoy working with the content! 😊
