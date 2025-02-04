---
layout: article
title: 🎮Analyzing Gaming Behavior
abstract: Streamlit App_Machine Learning Tool To Predict Gaming Engagement Level
categories: Demo
tags: demo Streamlit ML
eyeCatcher: https://raw.githubusercontent.com/PhuongFX/jekyll-theme-antarctica/1/assets/img/Screenshot%202024-09-04%20120353.jpg
---

---


**Gaming Engagement Prediction**
=====================================

Are you curious about what makes gamers tick? 🤔 Do you want to know how to predict their engagement levels? 📊 Well, you're in the right place! 😊 This project aims to predict the engagement level of gamers based on various factors such as age, gender, location, game genre, playtime hours, and more.

**`DEMO:`🎮GamerDNA!** [![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://ml-online-gaming-lvpredict.streamlit.app)
==========================
Streamlit App_Machine Learning Tool To Predict Gaming Engagement Level


<div style="text-align: left;">

  <a href='https://github.com/PhuongFX/ButterFlySpace/blob/main/LICENSE'><img style='display: inline-block; margin: 0; padding: 0;' src='https://img.shields.io/badge/License-AGPL%203.0-blue.svg' alt='License: AGPL-3.0'></a>
  <a href='https://www.python.org/'><img style='display: inline-block; margin: 0; padding: 0;' src='https://img.shields.io/badge/Python-3.x-blue' alt='Python'></a>  
  <a href='https://streamlit.io/'><img style='display: inline-block; margin: 0; padding: 0;' src='https://img.shields.io/badge/Streamlit-1.36.0-orange.svg' alt='Streamlit'></a>
  <a href='https://www.tensorflow.org/'><img style='display: inline-block; margin: 0; padding: 0;' src='https://img.shields.io/badge/TensorFlow-green.svg' alt='TensorFlow'></a>
  <a href='https://en.wikipedia.org/wiki/Machine_learning'><img style='display: inline-block; margin: 0; padding: 0;' src='https://img.shields.io/badge/Machine%20Learning-🤖-green.svg' alt='Machine Learning'></a>
  <a href='https://github.com/PhuongFX/Online-Gaming'><img style='display: inline-block; margin: 0; padding: 0;' src='https://img.shields.io/badge/Open%20Source-%E2%9D%A4-green.svg' alt='Open Source'></a>
  <a href='https://www.kaggle.com/datasets/rabieelkharoua/predict-online-gaming-behavior-dataset'><img style='display: inline-block; margin: 0; padding: 0;' src='https://img.shields.io/badge/Dataset-📊-red.svg' alt='Dataset'></a>
  
</div>


> A machine learning-based application designed to analyze online gaming behavior and predict player engagement levels.

> This application is intended to assist game developers in identifying players at risk of churn and creating personalized experiences to increase player satisfaction and loyalty.

<p align='center'>
  <img src="https://raw.githubusercontent.com/PhuongFX/jekyll-theme-antarctica/1/assets/img/Screenshot%202024-08-19%20203100(1).jpg"/>
</p>


## `How it Works` 🫶

### Step 1: Select the Features

* Choose the characteristics that describe the player and the game 📝.
* Select the features that are relevant to your analysis.

### Step 2: Click the 'Predict' Button

* Get the predicted engagement level of the player 📊.
* Use the predicted engagement level to create personalized experiences for the player.

### Step 3: Get the Results

* Use the app to predict player engagement levels for note-taking, research, or content creation 📝.


## `Dataset` 📊


Containing 40,034 samples and 13 features. Here's a sneak peek at what's inside:

* `PlayerID`: Unique identifier for each player
* `Age`: Age of the player
* `Gender`: Gender of the player (Male/Female)
* `Location`: Location of the player
* `GameGenre`: Genre of the game played (Strategy, Sports, Action, RPG, Simulation)
* `PlayTimeHours`: Number of hours played
* `InGamePurchases`: Number of in-game purchases made
* `GameDifficulty`: Difficulty level of the game (Easy, Medium, Hard)
* `SessionsPerWeek`: Number of sessions played per week
* `AvgSessionDurationMinutes`: Average duration of each session in minutes
* `PlayerLevel`: Level of the player
* `AchievementsUnlocked`: Number of achievements unlocked
* `EngagementLevel`: Engagement level of the player (Low, Medium, High)


## `Architecture` 🤖

Here's a step-by-step guide to how to approached this project:

1. **Data Preprocessing 🧹**: Removing missing values, encoding categorical variables, and scaling numerical variables.
2. **Exploratory Data Analysis (EDA) 🔍**: Exploring the dataset to understand the distribution of each feature and their relationships.
3. **Modeling 🤖**: Training and evaluating several machine learning models to predict the engagement level of gamers. The models used include:
	* Logistic Regression
	* K-Nearest Neighbors
	* Support Vector Machines
	* Decision Tree
	* Random Forest
	* AdaBoost
	* Gradient Boosting
	* Naive Bayes
	* Neural Network
	* XGB
	* HistGradientBoostingClassifier
	* LGBMClassifier
	* CatBoostClassifier
	* ExtraTreesClassifier
4. **Hyperparameter Tuning 🔧**: Tuning hyperparameters using Bayesian optimization to improve the performance of the models.

## `Results` 📊

The best performing model was the XGB model with an accuracy of 91.64% on the test set.

| Model | Training Accuracy | Test Accuracy |
| --- | --- | --- |
| XGB | 93.39% | 91.64% |
| RandomForest | 92.12% | 91.42% |

## `Fine Tuning` 🔧
--------------

<p align='center'>
  <img src="https://github.com/PhuongFX/OnlineGame/blob/main/newplot.png" />
</p>

--------------
Predicting gamer engagement is a complex task, but with the right approach and techniques, we can achieve high accuracy. 📈 This project demonstrates the power of machine learning in understanding gamer behavior and predicting their engagement levels.

## `Example Use Cases`

* Analyze online gaming behavior to identify patterns and trends.
* Predict player engagement levels to inform game development and marketing strategies.
* Use the application to identify areas for improvement in game design and player experience.


## `🙅‍♂️Disclaimer`

> This app is licensed under AGPL-3.0 License and is for personal use only and should not be used for commercial purposes.
The GamerDNA model is a pre-trained model and may not always produce accurate results.


## `Get Involved!` 😌
I hope you found this project informative and engaging! 😊  
If you're interested in collaborating and contributing to the project, please let me know! I'd love to hear from you.
* [Follow me on GitHub](https://github.com/PhuongFX)
* [Follow me on Hugging Face](https://huggingface.co/PhuongFX)



## `Getting Started` 🚀

To get started with this project, you'll need to:

* Install the required libraries, including TensorFlow, Keras, and OpenCV 📦
* Download kaggle datasets using `download -d gpiosenka/butterfly-images40-species` 📈
* Run the code to train and evaluate the model 🤖

Enjoy working with the content! 😊
