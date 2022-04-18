# Caption Generator
IMAGE CAPTIONING is the task of generating textual descriptions of a given image, requiring techniques of **COMPUTER VISION** and **NATURAL LANGUAGE PROCESSING**. <br>


<img alt="image_caption_problem" src="https://user-images.githubusercontent.com/98893201/163872860-765beb59-e8eb-4bcc-9a40-045a97806c66.png">

It is a process of recognizing the context of an image and annotating it with relevant captions with the help of datasets provided during model training. <br>
For this purpose, we need to process both the language or statements and the images. For the Language part, we use recurrent Neural Networks (RNN) and for the Image part, we use Convolutional Neural Networks (CNN) to obtain the feature vectors respectively. In this case, the features of each image will be extracted by a CNN encoder which uses a pre-trained ResNet model provided by Pytorch. <br>
The extracted features will be fed to a LSTM decoder which in turn generates a possible image caption. MS-COCO is one of the most used datasets for this purpose. <br>

The [jupyter notebook](Image_caption_project.ipynb) available in this repository covers the following topics:
- Exploring COCO dataset
- Preprocessing images and captions
- Encoder: pre-trained CNN with ResNet 152
- Decoder: LSTM for training and testing
- Rouge_L metrics 
- Coco Evaluation toolkit 
