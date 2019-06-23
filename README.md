# Skin-Lesion-Classification
+ Melanoma vs Others classification of skin lesions obtained from ISIC dataset with an imbalanced dataset of size 2000 images.
+ The dataset contains 374 melanoma images (class 1), and 1626 other images (class 2).
+ Split train/val/test 60/20/20
+ Oversampling or SMOTE analysis gave better results, however due to the constraints provided done without oversampling.
+ Used encoder decoder UNET architecture for predicting the segmenation masks for the ground truth lesion images.
+ PS: I have used pickle to save my processed dataset as a list, which consumes more memory. Recommend using numpy arrays and npz for saving the dataset locally before uploading on cloud environment as for Colab the RAM being offered is 12 GB and with 2000 x 256 x 256 x 3 images, you are surely gonna runout of memory and thereby restarting your session every time.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

```
Anaconda
pip
Google Colab
Keras
TensorFlow
```


## Built With

* [Colab](https://colab.research.google.com) - Cloud jupyter notebook, offering free service upto 8GB RAM and 48GB HDD.


## Authors

* Mohammed Khursheed Ali Khan


## Acknowledgments

* [UNET Architecture paper](https://arxiv.org/pdf/1505.04597.pdf)
