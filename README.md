# Gaze360-Tensorflow

This is an unofficial imprlemntaion of the paper: [Gaze360: Physically Unconstrained Gaze Estimation in the Wild](http://gaze360.csail.mit.edu/)

## Status

As I found that the images in the orginal dataset are all underexposed, and thus, will not generlaize to new datasets, I'm currently working on data argumentation. 

In the paper the authors used [DensePose](https://github.com/facebookresearch/Densepose) for body and head detection. However, as the dataset provided by the authors only include hads and not the full sence this makes not a lot of sence anymore. Moreover, DensePose is outdated and not well supported anymore. Thus, currently I'm suing [dlips](http://dlib.net/python/index.html) CNN face detection model. The drawback here is, that this model can not finde the head when the human is not faceing the camea.

## Dependencies
* Python3.6+
* TensorFlow 2.0+
* dlib1 9.17.0+
* tqdm


## Dataset:
Please get the dataset direcly from the authors of the original paper, [here](http://gaze360.csail.mit.edu/download.php).
