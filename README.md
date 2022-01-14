# pytorch
Unets, auto-encoder, classifier for 2D/3D image analysis

AutoEncoder:  Similar to a Unet but with the skip connections removed.  This learns an underlying latent space for the input images that can then be used for a 
compressed representation.

AutoEncoder_UMAP:  This takes the latent space representations from the Autoencoder and performs UMAP analysis on it.

Classifier_3D:  A traditional convonet with the 3rd dimension in channel space for performing image classification.

DeepFijiv2.ijm:  This takes a folder of images and corresponding ImageJ roi zip files and generates training data for the Unets below.

Unet_2D:  A pytorch based Unet for performing segmentation.  The training data is expected to be x+2 channels.  Where x is the number of input channels, and the remaining two are 
to be learned.  Typically these are binary channels filled in object and the outline of that object.

Unet_3D:  The same but adapted to 3D.

