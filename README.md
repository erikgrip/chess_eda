# chess_prediction

## Table of contents
* [General info](#general-info)
* [Technologies](#technologies)
* [Setup](#setup)
* [Input](#input)
* [Output](#output)

## General info
The purpose of this project is to train a model that predicts chess games. The process from exploratory data analysis (EDA) to the export of a fitted logistic regression classifier can be followed in a series of notebooks created in Jupyter Lab.

## Technologies
Project is created with:
* Jupyter Lab
* Scikit Learn
* Logistic Regression
* Random Forest
* Pandas
* Seaborn and Matplotlib
* Docker

## Setup
This project can be viewed by opening the Jupyter notebooks in the /notebooks folder.
1. [Exploratory Data Analysis](https://github.com/erikgrip/chess_prediction/blob/main/notebooks/1_exploratory_data_analysis.ipynb)
2. [Problem Definition](https://github.com/erikgrip/chess_prediction/blob/main/notebooks/2_problem_definition.ipynb)
3. [Train/Test Split](https://github.com/erikgrip/chess_prediction/blob/main/notebooks/3_train_test_split.ipynb)
4. [Feature Exploration](https://github.com/erikgrip/chess_prediction/blob/main/notebooks/4_feature_exploration.ipynb)
5. [Model Training](https://github.com/erikgrip/chess_prediction/blob/main/notebooks/5_model_training.ipynb)

To run the notebooks though, you need Docker and Docker Compose. See official docs [here](https://docs.docker.com/compose/install/) for instructions on how to install. With Docker and docker-compose installed, clone the repository using a local terminal.
```
$ git clone https://github.com/erikgrip/chess_prediction.git
```

Then navigate into the project folder and run:
```
$ docker-compose up -d
```
Once the Jupyter notebook container is running the notebooks are accessed by navigating to http://localhost:8888/lab/tree/work/notebooks in a web browser. Enter 'easy' when promted for a token.

## Input
The training data can be found in the /data directory. It was downloaded from [Chess.com](https://www.chess.com) using [chess_dashboard](https://erikgrip.github.io/chess_dashboard/).
The data contains the game history for the player 'gripklo', which is my own alias.

## Output
The output of the project is a model file, saved in the /model directory.
