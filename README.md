# Facial Keypoints Detection

Effects of working with Facial Keypoints Detection dataset from Kaggle competition (link in Resources below). Projects include data preprocessing, model training, evaluating and improving model's parametrs with Hyperas package.



## Authors

- [@gwiazale](https://github.com/gwiazale)


## Installation

Firstly, download dataset according to a instruction in URL in Data sources section of this README.
Next, install Facial-Keypoints-Detection with npm after downloading it to your computer, unzipping it and open a project folder in your terminal.

```bash
  npm install Facial-Keypoints-Detection
```
After that, just open it in your favourite enviroment.    
## Data sources

 - [Source of the dataset](https://www.kaggle.com/competitions/facial-keypoints-detection/data)


## Code structure

1. Import packages
2. Data preparation:
- Loading data
- Describing data
- Describing new datasets after fixing null values
    - Filling null values with mean value for each column in DataFrame
    - Deleting rows with null values
    - Deleting columns, where percentage of null values are greater than 1%, rest is filled with mean value of the column
- Results of fixing null values
    - Filling null values with mean value for each column in DataFrame
    - Deleting rows with null values
    - Deleting columns, where percentage of null values are greater than 1%, rest is filled with mean value of the column
3. Models for:
- Filling null values with mean value for each column in DataFrame
    - Model evaluation
- Deleting rows with null values
    - Model evaluation
- Deleting columns, where percentage of null values are greater than 1%, rest is filled with mean value of the column
    - Model evaluation
Parametrs of the models were improved with my Google Colab project, where is a script of choosing best params using Hyperas package.
4. Submission results


## Results and evaluation

Results of training and validating the first model:

![ScreenShot](Results of model 1.png?raw=true "Results of model 1")

Predicting (x, y) locations of eyes, nose and mouth for the first model performs:

[Predictions of model 1.png](https://github.com/gwiazale/Facial-Keypoints-Detection/blob/e5d663a053a7193d24f7b101c8b23c02e8d3b14e/Predictions%20of%20model%201.png)

Results of training and validating the second model:

![ScreenShot](Results of model 2.png?raw=true "Results of model 2")

Predicting (x, y) locations of eyes, nose and mouth for the second model performs:

![ScreenShot](Predictions of model 2.png?raw=true "Predictions of model 2")

Results of training and validating the third model:

![ScreenShot](Results of model 3.png?raw=true "Results of model 3")

Predicting (x, y) locations of eyes, nose and mouth for the third model performs:

![ScreenShot](Predictions of model 3.png?raw=true "Predictions of model 3")

## Future work

Proposition to improve the predictions are:
- improving model architecture
- choosing another way to data preprocessing (e.g. data augmentation for the second dataset, choose another solution to filling null values than mean value of the feature).



## Resources

 - [Code of Nagasai user of Kaggle community](https://www.kaggle.com/code/nagasai524/facial-keypoint-detection-using-cnn#Future-Scope)
 - [Code of Diaa Eldiyn Essam user of Kaggle community](https://www.kaggle.com/code/diaaessam/face-landmarks-detection#Architecture-2)
 - [A guide to an efficient way to build neural network architectures- Part I](https://towardsdatascience.com/a-guide-to-an-efficient-way-to-build-neural-network-architectures-part-ii-hyper-parameter-42efca01e5d7)
 - [A guide to an efficient way to build neural network architectures- Part II](https://towardsdatascience.com/a-guide-to-an-efficient-way-to-build-neural-network-architectures-part-i-hyper-parameter-8129009f131b)
 - [How to deal with Missing Values in Machine Learning](https://medium.com/geekculture/how-to-deal-with-missing-values-in-machine-learning-98e47f025b9c)
