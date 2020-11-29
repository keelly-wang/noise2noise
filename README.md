# Noise2Noise for PyJAMAS
Adapted from Noise2Noise: Learning Image Restoration without Clean Data - Official TensorFlow implementation of the ICML 2018 paper

Confocal microscope images of Resille:GFP, a basal-lateral cell membrane marker, in stage 14 *Drosophila Melanogaster* embryos can provide valuable information about cell shape and volume changes during morphogenetic processes. However, automated image segmentation methods (e.g. watershed) do not perform well on these images due to their low signal-to-noise ratio. The goal is to create a ML denoising plugin for PyJAMAS specific to Resille:GFP. This workflow can potentially be applied to other markers as well. 

## To-do list:
1. Quantify and model microscope noise - Gaussian? Poisson? Bernoulli?
2. Adapt .tfrecords creation code to bundle together pairs of noisy images.
3. Train model on sample .jpg images, and validate visual effects of trained model.
4. Modify training and validation code to be compatible with lossless multipage .tiff images.
