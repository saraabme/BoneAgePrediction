# Bone Age Prediction

This notebook explores the dataset used in the Pediatric Bone Age Challenge, 2017, commonly known as the RSNA(Radiological Society of North America), and attempts to predict the ages of children using X-ray images of their hands. More information about the dataset as well as the dataset itself can be found on Kaggle <a href = 'https://www.kaggle.com/kmader/rsna-bone-age'>here.</a><br>

## Background information
A bone age study helps doctors estimate the maturity of a child's skeletal system. This is done by taking a single X-ray of the left wrist, hand, and fingers. The bones on the X-ray image are compared with X-ray images in a standard atlas of bone development. The atlas is based on data from many other kids of the same gender and age. The bone age (also called the skeletal age) is measured in years.

Children’s bones have areas of new bone growth called growth plates at both ends. They add length and width to the bone. They can be seen on an X-ray because they're softer and contain less mineral, making them appear darker on an X-ray image than the rest of the bone.

Bones and growth plates change over time. As kids grow, their growth plates look thinner on X-rays and eventually disappear (called "closed growth plates"). Doctors assign a child’s bone age based on which standard X-ray images in the atlas most closely match how the child's bones look on the X-ray.

The current method of determining bone age in children using X-rays has several limitations and challenges. Traditionally, radiologists manually assess X-ray images by comparing them to reference atlases or standards to estimate a child's skeletal maturity. However, this process is subjective and can be prone to inter-observer variability, leading to inconsistencies and inaccuracies in age estimation. Additionally, this method relies heavily on the expertise and experience of the radiologist, making it time-consuming and potentially costly.

In contrast, leveraging deep learning models, such as the pre-trained Xception model, offers a promising solution to enhance the accuracy and reliability of bone age determination from X-ray images. Xception is a convolutional neural network (CNN) architecture known for its exceptional performance in image classification tasks.

By utilizing transfer learning techniques, we can fine-tune the pre-trained Xception model on a large dataset of labeled X-ray images with corresponding bone age annotations. This allows the model to learn intricate patterns and features indicative of skeletal maturity directly from the data, bypassing the limitations of manual assessment.


## Model description
The notebook uses the pre-trained model Xception to predict ages. The ImageDataGenerator class from Keras has been used to enable efficient loading, preprocessing, and augmentation of the dataset. The model obtained a mean absolute error of approximately 7.6 months.<br>
## Requirements
<ul>
  <li> <b>Tensorflow:</b> To use Xception and related functions for training and preprocessing</li>
  <li><b> Numpy:</b> To work with the dataset</li> 
  <li><b> Pandas:</b> To load CSV files and plot data</li>
  <li><b> Matplotlib:</b> To create visualisations</li>
  <li><b> Seaborn:</b> To create visualisations</li>
  <li><b>Sklearn:</b> To split data into training and validation</li>
  </ul>
  
## Results
<img src ='Results.png'></img>
  
