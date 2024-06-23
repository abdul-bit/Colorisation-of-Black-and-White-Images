
# Colourisation of GrayScale Images for Wildlife Tracking

**_Abstract -_** The project aims to colorize grayscale images
using Image Processing, Machine Learning, and Deep Learning
techniques. Colorizing an image is one such problem that
doesn’t have a clear-cut solution or approach. A wide range
of authors have developed novel Convolution based approaches,
Auto-Encoder-based models and so on for the same. This project
aims to enhance images using Filtering, Feature Extraction,
Color Space mapping to effectively model the data being passed
to a Deep Learning Model to colorize the image.


## Authors

- [Abdul Rahman Shigihalli](https://www.github.com/abdul-bit)
- [Aanchal Narendran](https://github.com/aanchal-n)
- [A Narendiran](https://github.com/naren951)
- [Abhishek D](https://github.com/abhishekd23)


## Introduction
Image colorization involves using a wide range of statistical models to estimate the red, green and blue values of
pixels in a grayscale image. There is an ever-present research
intrigue in the field of colorisation owing to its open-ended
nature. Most photographic solutions between 1826 - 1980 have
relied on capturing their images in Grayscale. Colourizing
these images is similar to art restoration. Although old, they
are of importance and hold sentimental, historical value, and
scientific value. CCTV solutions over the past decades are
usually recorded in grayscale images. Effectively limiting the
usage of these cameras in identifying vehicles and people
of interest in legal cases. Although luminance and grayscale
help isolate information regarding the objects in the image,
color helps improve the quality of information obtained from
grayscale images. This project aims to develop a solution to
aid in colourizing images in one such domain.

## Dataset
The dataset ”Animals 151” is used in this project. It
contains RGB pictures of about 151 animals, with each animal
having anywhere between 30 to 60 images. Each image is of
the size 224x224 pixels ??. One of the working assumptions
of this project is that these color images will be able to
effectively model the actual scenario. Most animals are found
in the wild and are often captured from varied backgrounds.
We hope that with effective feature detection and modeling
the solution effectively catches any animals of interest in
the frame. For the sake of this project, subject to compute
restraints the dataset size has been constricted to 60 animals
instead of the original 151.

## Experimental Results



### XGBoost Regressor

| Image                  | Chi-Square | InterSect |
|------------------------|------------|-----------|
| Ailurpoda-melanoleuca  | 11037      | 0.308     |
| Ceratotherium-Simum    | 7548       | 1.67      |
| Dasypus-Novemcinctus   | 4.8        | 0.36      |

![image](https://github.com/abdul-bit/Colorisation-of-Black-and-White-Images/assets/59999587/440ccd2b-a0af-4967-875a-0753a0ae0fd7)


### Convolutional Neural Network

| Image                  | Chi-Square | InterSect |
|------------------------|------------|-----------|
| Ailurpoda-melanoleuca  | 60.4       | 1.5       |
| Ceratotherium-Simum    | 40.03      | 0.9       |
| Dasypus-Novemcinctus   | 53.06      | 1.59      |

![image](https://github.com/abdul-bit/Colorisation-of-Black-and-White-Images/assets/59999587/b1cde331-7c7a-42f3-9ac0-bc8d4f1c0599)

### Auto Encoder

| Image                  | Chi-Square | InterSect |
|------------------------|------------|-----------|
| Ailurpoda-melanoleuca  | 2.04       | 1.8       |
| Ceratotherium-Simum    | 0.6        | 2.6       |
| Dasypus-Novemcinctus   | 2.4        | 0.38      |

![image](https://github.com/abdul-bit/Colorisation-of-Black-and-White-Images/assets/59999587/4bc115b7-0754-400d-9276-6264f55f7d05)

## Contributions

1) **Aanchal Narendran :** XGBoost Regression with K-Means quantisation.
2) **Abdul Rahman Shigihalli :** AutoEncoders.
3) **A Narendiran :** Convolutional Neural Networks. 
4) **Abhishek Dinesh :** Convolutional Neural Networks: 


## References


- **R. Pucci, C. Micheloni, N. Martinel**
_“Collaboration among Image and
Object Level Features for Image Colourisation.”_ , ArXiv, 2021.

- **R. K. Gupta, A. Y. Chia, D. Rajan, E. S. Ng, H. Zhiyong**
 _“Image Colorization Using Similar Images”_, Proceedings of the 20th ACM international conference on Multimedia, 2012.
- **M. G. Blanch, M. Mrak, A. F. Smeaton, N. E. O’Connor**
_“End-to-End Conditional GAN-based Architectures for Image Colourisation”_ , arXiv. 2019.
- **H. J. Kim, Y. D. Eo, D. K. Seo, J. S. Park, G. W. Park, W. Y. Park**
_"Automatic Colorization of Grayscale Aerial Imagery Using XGBoost
Regression”_, Proceedings of 40th Asian Conference on Remote Sensing, 2019.
