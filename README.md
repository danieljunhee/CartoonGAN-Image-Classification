# CartoonGAN-Image-Classification

In this project, we deal with the task of classifying cartoonized images. Cartoonizing a given real-world photo can be done via the CartoonGAN model (paper link: https://openaccess.thecvf.com/content_cvpr_2018/papers/Chen_CartoonGAN_Generative_Adversarial_CVPR_2018_paper.pdf). This is a type of GAN that was specifically designed and trained to modify real-world images as cartoon style.

Now let's consider the task of classifying an image as 'dog' or 'cat'. We can imagine that for humans, the level of difficulty of classifying a real-world dog image as a dog and the level of difficulty of classifying a cartoonized dog image as a dog would be pretty similar (and similarly for cats).

The question of our interest is: "Does this also hold for image classification models?"

More specifically,
- If we train an image classification model with cartoonized images (as a binary classification of dogs and cats), how well will it perform on classifying real-world images of dogs and cats? (TRAIN & VALIDATION: cartoonized images, TEST: real-world images)
- If we train an image classification model with real-world images (as a binary classification of dogs and cats), how well will it perform on classifying cartoonized images of dogs and cats? (TRAIN & VALIDATION: real-world images, TEST: cartoonized images)

[Dataset Citation]
- Oxford-IIIT Pet Dataset
  - Cats and Dogs \
  Parkhi, O. M. and Vedaldi, A. and Zisserman, A. and Jawahar, C.~V. \
  IEEE Conference on Computer Vision and Pattern Recognition, 2012
