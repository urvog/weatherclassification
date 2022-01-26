# Weather Image Classification with Keras

Weather phenomenon recognition notably affects many aspects of our daily lives, for example, weather forecast, road condition monitoring, transportation, agriculture, forestry management, and the detection of the natural environment. In contrast, few studies aim to classify actual weather phenomenon images, usually relying on visual observations from humans.

In this project we propose a study weather classification from images using Convolutional Neural Networks (CNNs) with Keras+Tensorflow. We present a dataset with 3348 images with six weather conditions (rain, shine, sunrise, fogsmog, snow, cloudy) obtaining a precision of 90% in the validation data and 87% in test data. Realizing the automatic and high-quality classification of weather phenomena images can provide a reference for future research on weather image classification and weather forecasting.

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

![image](https://user-images.githubusercontent.com/459689/151182165-bb84cdb9-35a0-42a5-9f0c-bbbc6b0eb4e5.png)

Validation Dataset Distribution

![image](https://user-images.githubusercontent.com/459689/151178807-358975ef-0170-42c9-a2d4-96b83229f690.png)

Test Dataset Distribution

![image](https://user-images.githubusercontent.com/459689/151178822-7ee75d3b-90cc-4551-97d5-e556ea22dda6.png)

## Image Samples
Cloudy

![image](https://user-images.githubusercontent.com/459689/151182218-e8e4a38e-9f4c-4994-bf7e-67daaa7fb069.png)

Rain

![image](https://user-images.githubusercontent.com/459689/151182240-e50e52ce-cad4-470c-841c-57d59fd099a0.png)

Sunrise

![image](https://user-images.githubusercontent.com/459689/151182332-2bd75867-96d7-45a7-bb22-5d6525c49236.png)

## Image processing and Data Augmentation
At this stage we are going to generate images using Keras Generator, in this way we can see how the Data Augmentation strategy is working. We disable rescaling so that images can be easily viewed.

![image](https://user-images.githubusercontent.com/459689/151182590-2788bec7-1737-4a9b-bc0a-85785f1e5fe0.png)
![image](https://user-images.githubusercontent.com/459689/151182624-0c2c61ce-bdee-419e-90c5-8e9a9339be78.png)


## Model Implementation

The strategy for this work is to make two models from scratch and one using transfer learning, in this way we can see the behavior and performance of each one.

### Model 1

![image](https://user-images.githubusercontent.com/459689/151182770-f160905c-cf65-45dd-ad7b-e2efd11f92dd.png)


### Model 2

![image](https://user-images.githubusercontent.com/459689/151182799-90944ec1-3a3e-4406-b9f4-91182b24cd77.png)

### Model 3 with Transfer Learning

![image](https://user-images.githubusercontent.com/459689/151182987-d89d3f0c-d8f9-463b-a13f-b94a5a311d4e.png)
![image](https://user-images.githubusercontent.com/459689/151182974-b1a20c7d-1c2c-4f5d-86ac-a7fb9b07d0aa.png)

## Scores

### Model 1

![image](https://user-images.githubusercontent.com/459689/151183351-4d712129-39eb-4c3f-91e4-66649f3ee38e.png)

### Model 2

![image](https://user-images.githubusercontent.com/459689/151183380-cee3758b-16f6-45f4-8292-372a13ea2f08.png)

### Model 3

![image](https://user-images.githubusercontent.com/459689/151183437-6c075b81-8f97-430c-bd18-0426e0a585d9.png)






