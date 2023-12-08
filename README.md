<h2>ABOUT</h2>

<p>This repo consists of 4 branches till now.</p>

<li><b>Main</b> : I extracted this code from Nitin's YT channel and it gave some error, which I was not aware of so I gave up on this code and started looking for other tutorials. I looked at this code after going through many tutorials and realised that it is very similar to the ML mastery code that I understood and started implementing in the new branches.</li>

<li><b>ml-mastery-br-1</b> : This code I took from the ML Mastery tutorial. I have identified the follwing mistakes in this code :
<ul>In the image feature extraction function - the line where I was supposed to remove the last layer from VGG model to only consider the features and not the class weights I removed model.layers[-1].output which gives the class weights and not the features, It should have been model.layers[-2].output</ul>
<ul>The dataset in this code is the one which I had downloaded from another source and did not have internal splits in train - development- test so the code got stuck there.</ul>
</li>

<li><b>ml-mastery-data-split</b> : In this code I tried to split the data by myself using the os function in python, i tried many times but it was not working. So I finally decided to follow the tutorial completely and download their dataset which was already split into train-test-development directories
<i>This might also have the VGG layer mistake</i>
</li>

<li><b>custom-dataset-ml-mastery</b> : In this I downloaded the dataset from tutorial and started the same process again </li>

<h2>DATASET</h2>
The dataset being used in all the branches is Flickr8k dataset
It consists of 6k training images
1k validation images
1k testing images
Every image has 5 corresponding captions to it.
The model used is VGG-16 pretrained model - <u>Visual Geometry Group</u>
16 represents the # of weight layers in the model.
It is a CNN based model containing 3X3 convolutional layers stacked on top of each other in increasing depth.

<h2>RESOURCES</h2>
More advanced model will be Resnet which can be trained upto 200 layers deep.
<a href="https://www.youtube.com/@ManifoldAILearning">youtube tutorial to learn DL in depth</a>
<a href="https://www.youtube.com/watch?v=sz-hCpuAFYY&list=PL12YWfULs0pnL_9Pj6udM6PE2-SWZbTlX&index=3">Tutorial for VGG-16 code</a>
The image_captioning_vgg.ipynb file code is taken from Nitin's Youtube channel - not from the link pasted above.
