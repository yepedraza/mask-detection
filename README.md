# Face mask detection

Through the use of convolutional neural networks, I made a model that it's capable of detecting by reading an image if a person is wearing a face mask or not. The database I'm using contains about 6400 images of people. Each of these images also has a JSON type file that indicates many of its characteristics, being "class_name" the one that indicates the types of accessories that the people in the image are wearing (where we're going to classify if they're wearing a mask or not). The objective of this project is to apply CNN for a possible tool that uses computer vision and artificial intelligence to prevent infections in closed spaces.

## Building model

I created a [notebook](https://github.com/yepedraza/mask-detection/blob/d3ebf0175d6646432f8901c95325125fa8c61bf8/maskDetection.ipynb) where I do the data preprocessing and model building. It is important to identify the characteristics of the dataset and the transformations that I applied:
  * Class name extract by JSON file
  * Data separation and normalization (124x124 size)
  * Data augmentation with ImageDataGenerator from keras image preprocessing
  * Use of scikit-learn for data treatment
  
The model architecture is the following:

<img align="center" alt="classd" src="https://github.com/yepedraza/mask-detection/blob/d3ebf0175d6646432f8901c95325125fa8c61bf8/img/model.png" />
<br>

The model has 23M training parameters aprox and you can download it [here](https://drive.google.com/file/d/1oLV40ere7hftzJzp2v2hInLxv9cE90i0/view?usp=sharing)

---
*Made by @yepedraza* 
