# Visualizing Weights of CNN Deep learning model on ISIC dataset: Project overview
* I have visualized the intermediate weights that exist between the layers of a neural network
* An image from the data set below fed into the network
* Output is an image representing 'weight concentrations'
## EDA

![alt text](https://github.com/nins15/Visualizing-Weights-of-CNN-model-on-ISIC-dataset/blob/master/Disease.png "Disease")
![alt text](https://github.com/nins15/Visualizing-Weights-of-CNN-model-on-ISIC-dataset/blob/master/Height_width.png "Size")
![alt text](https://github.com/nins15/Visualizing-Weights-of-CNN-model-on-ISIC-dataset/blob/master/Sampleimages.png "sampleimages")
Solutions:
To display a image representing weight concentration means to show that on which part is the layer is focusing
so first run the kerastrainingtesting then run the trainandvisualize.
We have used 3 convolution layers and one fully connected layer.
Observation:
The first layer acts is retaining the full shape of the image, although there are several filters that are not activated and are left blank. At that stage, the activations retain almost all of the information present in the initial picture.
 As we go deeper in the layers, the activations become increasingly abstract and less visually interpretable. They begin to encode higher-level features. Higher presentations carry increasingly less information about the visual contents of the image, and increasingly more information related to the class of the image.
As mentioned above, the model stucture is overly complex to the point where we can see our last layers actually not activating at all, there's nothing more to learn at that point.

