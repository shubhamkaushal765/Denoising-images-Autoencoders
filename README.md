# Machine Learning Projects - by Shubham Kaushal

## Denoising images | Autoencoder | CNN model
Dataset <br>
NoisyOffice is a multivariate dataset hosted by the UC Irvine ML repository. It consists of 54 images of clean documents and 216 images of tampered documents (noise is introduced in four different ways). The task is to design an autoencoder using convolutional neural networks (CNNs), to be able to eliminate the different noises in the images (denoising). Here I have built two different models: the first one is a basic CNN with one encoding layer, one decoding layer followed by an output layer. The second one is deep CNN with three encoding and three decoding layers followed by an output layer.

Preprocessing <br>
<ul>
  <li>Each noisy image is named as :	FontABC_NoiseD_EE.png <br>
where FontABC: name of the font; NoiseD: type of noise; EE: TR->Training set, TE->Testing set, VA-> Validation set
  <li>Mapping of the noisy images to the clean images to create a (X and y) dataset.
</ul>

Developing Autoencoders
<ul>
  <li>Basic Autoencoder:    10 epochs, loss=0.508, val_loss=0.483
  <li>Adam Autoencoder:     5 epochs, loss=0.597, val_loss=0.513
  <li>RMSprop Autoencoder:  5 epochs, loss=0.278, val_loss=0.292
  <li>SGD Autoencoder:      5 epochs, loss=0.625, val_loss=0.612
</ul>

Final Model <br>
Optimizer: RMSprop (based on the loss parameter, binary_crossentropy) <br>
Epochs = 10, loss = 0.134, val_loss = 0.144 <br>
For more improvements, one can try getting more training data, data augmentation, building more complex/deeper models or try other optimizers.
<!-- 
For more improvements <br>
<ul>
  <li>More Training data
  <li>Data Augmentation
  <li>More complex/deeper model
  <li>Other Optimizers
-->
