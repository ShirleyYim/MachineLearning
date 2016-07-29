#Convolutional Neural Networks for image recognition

[CS231n: Convolutional Neural Networks for Visual Recognition](http://cs231n.stanford.edu/syllabus.html)   
Class taught by Andrej Karpathy at Stanford. [videos](https://www.youtube.com/playlist?list=PLLvH2FwAQhnpj1WEB-jHmPuUeQ8mX-XXG) were taken down for [legal concerns](https://twitter.com/karpathy/status/727618058471112704?lang=en).   

###CNN Parameters and terminology

Types of hidden layers: convolutional layers, max pooling layers, fully connected layers.  

Convolutional Layers - layers that have filters (aka kernels) that are convolved around the image.  

Number of filters (aka kernels)

Size of filter (F) - typically odd square numbers. typical values are 3x3, 5x5, up to 11x11. The trend is toward smaller filters.  

Stride: steps to take moving the filter.

Max pool size: max pooling is when you take a section and subsample only the largest value in the pool.

Fully connected layers are normal hidden layers.  

### State of the art research papers
[ImageNet](http://www.image-net.org/) is a dataset of 1.2 million images with 1,000 labels.  

[Gradient-based learning applied to document recognition](http://yann.lecun.com/exdb/publis/pdf/lecun-98.pdf)  
LeCun et al., 1998 LeNet-5.  

[ImageNet Classification with Deep Convolutional Neural Networks](https://papers.nips.cc/paper/4824-imagenet-classification-with-deep-convolutional-neural-networks.pdf)  
Krizhevsky et al. (2012) AlexNet breakthrough paper for convolutional neural networks. top-1 and top-5 error rates of 37.5%
and 17.0%.  5 layers + max pooling layers. First use of Relu (rectified linear units)  

[Visualizing and Understanding Convolutional Networks](https://arxiv.org/pdf/1311.2901v3.pdf)  
Zeiler and Fergus, 2013 - ZFNet. 14.8% error rate (eventually got to 11% with company clarify)  

[VERY DEEP CONVOLUTIONAL NETWORKS FOR LARGE-SCALE IMAGE RECOGNITION](https://arxiv.org/pdf/1409.1556.pdf)  
Simonyan et al. 2014.  aka VGG. 16 - 19 layers. 3x3 convolutional filters. 7.3% error rate.   

[Deep Residual Learning for Image Recognition](https://arxiv.org/pdf/1512.03385v1.pdf)  
He et al., 2015 aka resnet. Up to 152 layers. 3.57% top 5 error on ImageNet Test set. Uses skip connections (residual net). That allows diminishes vanishing/exploding gradient problems that occur in deep nets.  