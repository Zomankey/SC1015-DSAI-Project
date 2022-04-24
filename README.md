# Detection of Covid-19 Pneumonia via Chest X-Rays

## Repository Contents
1. Full Notebook - [Multi_Class_COVID_Classification_Model_.ipynb](https://github.com/karthikstar/SC1015Project/blob/main/Multi_Class_COVID_Classification_Model_.ipynb) <br>
  This is our main project code containing the exploratory data analysis and models

2. Sample Model Walkthrough - [SampleModelWalkthrough.ipynb](https://github.com/karthikstar/SC1015-Project/blob/main/SampleModelWalkthrough.ipynb)<br>
  This is just a simple walkthrough to demonstrate how our model can predict chest X-ray images, based on the 3 classes - COVID, Viral Pneumonia, and Normal. For a more detailed explanation, please check out our Full Notebook in our GitHub repository.

3. Project Slides - [BCF1_SC1015_Chest X-Ray Classification_Slides.pdf](https://github.com/karthikstar/SC1015-Project/blob/main/BCF1_SC1015_Chest%20X-Ray%20Classification_Slides.pdf) <br>
  This is the slides we used for our mini-project.

## How to run the file
If you intend to re-run and execute the model, please do the following:
<ul> 
  <li> Open the <b> Multi_Class_COVID_Classification_Model_.ipynb </b> file in Google Colaboratory https://research.google.com/colaboratory/ </li>
  <li> Upload the kaggle.json file when prompted for it at the start:  </li>
  <ul> 
    <li> To use the Kaggle API, sign up for a Kaggle account at https://www.kaggle.com. Then go to the 'Account' tab of your user profile (https://www.kaggle.com/<username>/account) and select 'Create API Token'. This will trigger the download of kaggle.json, a file containing your API credentials. </li>
  </ul>
</ul>

If you intend to simply check out our model and visualise how it predicts the classes of the chest x ray images, please do the following:
<li> Open the <b> SampleModelWalkthrough.ipynb </b> file in Google Colaboratory https://research.google.com/colaboratory/ </li>

## About
This is a Mini-Project for SC1015 (Introduction to Data Science and Artificial Intelligence) which focuses on Lung X-Rays from the COVID-19 Radiography Database.

## Problem Definition
<ul> 
  <li> Are we able to predict if someone has Viral or COVID-19 pneumonia based on their Chest X-Ray? </li>
  <li> Which model would be best to predict it? </li>
</ul>
 
## Motivation
As COVID-19 becomes endemic, the strain on healthcare services worldwide intensifies, making it more difficult to manage & detect the serious complications of COVID-19. <br>

Thus, we built this image classification model that classifies Chest X-Ray images into 3 classes (normal, viral pneumonia and COVID-induced pneumonia) to replace the current, manual way of diagnosing pneumonia which is unnecessarily exhausting limited resources and time-consuming yet may not be highly effective due to the presence of inevitable human errors.

## Exploratory Data Analysis
<ol> 
  <li> Bar Graph showing Number of datapoints in each class </li>
  <li> Matrices </li>
  <ul>
    <li> Contrast between Average Images of each Class </li>
    <li> Eigenimages from Principal Component Analysis </li>
    <li> Image Value Distribution </li>
  </ul>
</ol>

## Models Used
<ol> 
  <li> Convolutional Neural Network (CNN) </li>
  <li> Transfer Learning — Inception V3 </li>
</ol>

## Conclusion
Lung X-rays are visibly different from their clarity, which increases from normal, viral to COVID-19. Thus, we should be able to classify them to a relatively high accuracy. <br>
Our CNN model achieved an accuracy of 84.8%, while our transfer learning model achieved an accuracy of 93.5%. <br>
Thus, we can conclude that the transfer learning model is more accurate.

## What did we learn from this project?
<ul>
  <li> Data Collection and Preparation </li>
    <ol type = "1">
      <li> Importing Dataset Kaggle API </li>
      <li> Checking for blank images using the Python Imaging Library (PIL) image colour </li>
      <li> Handling imbalanced datasets through undersampling </li>
      <li> Encoding Classes into the Data </li>
    </ol>
  <li> Exploratory Data Analysis </li>
    <ol type = "1" , start = "5">
      <li> Convert images into matrices through numpy and keras preprocessing </li>
      <li> How to find the Principle Components of a dataset through sklearn </li>
      <li> How to find the image value distribution graphs through seaborn </li>
    </ol>
  <li> Building Classifier Model </li>
    <ol type = "1", start="8">
      <li> Keras, Tensorflow </li>
      <li> CNN </li>
      <li> Transfer Learning through Inception V3 </li>
    </ol>
</ul>

## Possible Future Work
In the future, we could improve our classifier by:
<ul>
  <li> Improving the dataset </li>
    <ul>
      <li> Image Augmentation though Genetic Algorithm or Keras ImageDataGenerator </li>
      <li> Adopt oversampling </li>
      <li> Adding on more X-Ray images from other sources to classes with less data </li>
    </ul>
  <li> Using other pre-trained models for transfer learning </li>
    <ul> 
      <li> VGG16 </li>
      <li> ResNet </li>
    </ul>
  <li> Considering other factors </li>
    <ul>
      <li> Whether the patient has symptoms of COVID </li>
      <li> Whether the patient has any close contact with confirmed COVID-19 cases </li>
    </ul>
</ul>
     
## Contributors
BCF1
> Elangovan Karthikeyan [@karthikstar](https://github.com/karthikstar) — Machine Learning Models <br>
> Lam Wei Lin, Zoey [@ZoeyNTU](https://github.com/ZoeyNTU) — Exploratory Data Analysis <br>
> Lee Pei Yee — Data Preparation

## References
<ul>
  <li> https://www.kaggle.com/tawsifurrahman/covid19-radiography-database </li>
  <li> https://github.com/Kaggle/kaggle-api#:~:text=reporting%20any%20issues.-,API%20credentials,file%20containing%20your%20API%20credentials. </li>
  <li> https://www.kaggle.com/code/sana306/detection-of-covid-positive-cases-using-dl </li>
  <li> https://towardsdatascience.com/exploratory-data-analysis-ideas-for-image-classification-d3fc6bbfb2d2 </li>
  <li> https://towardsdatascience.com/exploring-the-mnist-digits-dataset-7ff62631766a </li>
  <li> https://slidesgo.com/theme/curie-breakthrough#search-virus&position-17&results-74 </li>
  <li> https://towardsdatascience.com/illustrated-10-cnn-architectures-95d78ace614d </li>
</ul>
