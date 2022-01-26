# Weather Image Classification with Keras

Weather phenomenon recognition notably affects many aspects of our daily lives, for example, weather forecast, road condition monitoring, transportation, agriculture, forestry management, and the detection of the natural environment. In contrast, few studies aim to classify actual weather phenomenon images, usually relying on visual observations from humans.

In this project we propose a study weather classification from images using Convolutional Neural Networks (CNNs) with Keras+Tensorflow. We present a dataset with 3348 images with six weather conditions (rain, shine, sunrise, fogsmog, snow, cloudy) obtaining a precision of 90% in the test data. Realizing the automatic and high-quality classification of weather phenomena images can provide a reference for future research on weather image classification and weather forecasting.

Required Libraries:
- Tensorflow
- Keras
- PIL
- Seaborn
- pandas
- numpy
- matplotlib
- os

## Importing Datasets

Multi-class weather dataset(MWD) for image classification is a valuable dataset used in the research paper entitled “Multi-class weather recognition from still image using heterogeneous ensemble method”. The dataset provides a platform for outdoor weather analysis by extracting various features for recognizing different weather conditions.

URL: https://www.kaggle.com/mauricioarancibia/weatherimgclass/download

Upload arhive.zip file to colab.
Unzip archive.zip

## Data Exploration Analysis (EDA)

In this section we will proceed to perform the exploration and analysis of the data.

Training Dataset Distribution
![image](https://user-images.githubusercontent.com/459689/151178762-0a090911-b645-4a49-bc29-7f3dbd51b9fc.png)

Validation Dataset Distribution
![image](https://user-images.githubusercontent.com/459689/151178807-358975ef-0170-42c9-a2d4-96b83229f690.png)

Test Dataset Distribution
![image](https://user-images.githubusercontent.com/459689/151178822-7ee75d3b-90cc-4551-97d5-e556ea22dda6.png)
