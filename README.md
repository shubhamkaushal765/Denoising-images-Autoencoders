# Machine Learning Projects - by Shubham Kaushal

## Denoising images | Autoencoder | CNN model
Dataset <br>
NoisyOffice is a multivariate dataset hosted by the UC Irvine ML repository. It consists of 54 images of clean documents and 216 images of tampered documents (noise is introduced in four different ways). <br>
The task is to design an autoencoder using convolutional neural networks (CNNs), to be able to eliminate the different noises in the images (denoising). Here I have built two different models: the first one is a basic CNN with one encoding layer, one decoding layer followed by an output layer. The second one is deep CNN with three encoding and three decoding layers followed by an output layer.

Preprocessing <br>
<ul>
  <li>Each noisy image is named as :	FontABC_NoiseD_EE.png <br>
where FontABC: name of the font; NoiseD: type of noise; EE: TR->Training set, TE->Testing set, VA-> Validation set
  <li>Mapping of the noisy images to the clean images to create a (X and y) dataset.
</ul>
