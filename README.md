
# 400k Augmented MNIST: Extended Handwritten Digits

![Augmented Examples](https://www.googleapis.com/download/storage/v1/b/kaggle-forum-message-attachments/o/inbox%2F17037041%2F971476ebbf4243cc02cf2985d72f5ded%2F400k%20Augmented%20MNIST%20cover%20image.png?generation=1742929388926405&alt=media)

## Overview

The **400k Augmented MNIST** dataset is an extended version of the classic MNIST handwritten digits dataset. By applying a variety of augmentation techniques, I have increased the number of training images to **400,000** - roughly 40,000 per digit label. This large and diverse training set is designed to significantly improve the robustness and generalization of models trained on it, making them less susceptible to overfitting and more resilient against adversarial perturbations.

## Dataset Structure

The dataset is organized into two main directories:

- **Augmented MNIST Training Set (400k):**  
  This directory contains 10 subdirectories, one for each digit label ("Label 0" through "Label 9"). Each subdirectory holds the corresponding JPEG images generated via augmentation. These images have been produced using techniques such as random rotation, shear, translation, scaling, reflection, spatial padding, Ben Graham transformation, Gaussian noise, salt-and-pepper noise, and random text overlay.

- **MNIST Validation Set (4k):**  
  This directory also contains subdirectories "Label 0" to "Label 9". However, the validation set consists solely of the original MNIST images (approximately 400 per label) that were not used for augmentation. This allows you to evaluate model performance on natural, unaltered digit images, providing a clear benchmark for generalization.

## How to Use This Dataset

1. **Training:**  
   Use the augmented training set to train your deep learning models. The 400k images offer a wide variety of conditions, helping your model learn robust features that generalize well.

2. **Validation:**  
   Evaluate your models on the validation set, which contains only the original MNIST images. This will help you measure performance on “natural” digits, ensuring that improvements in robustness do not come at the expense of real-world accuracy.

3. **Flexibility:**  
   You can also experiment with mixed training (combining augmented and original images) to study how different training strategies affect model robustness and accuracy.

## Augmentation Techniques Applied

The following augmentation functions were used to generate the extended dataset:

- **Random Rotation:** Randomly rotates images within a specified angle range.
- **Random Shear:** Applies slight shearing transformations.
- **Random Translation:** Shifts images horizontally and vertically.
- **Random Scale:** Zooms in or out on the images.
- **Ben Graham Transform:** Enhances image contrast and clarity using a weighted Gaussian blur.
- **Random Gaussian Noise:** Adds Gaussian noise to simulate sensor or environmental disturbances.
- **Random Salt-and-Pepper Noise:** Introduces random pixel-level corruption.
- **Random Text Overlay:** Places random, semi-transparent text on images to simulate artifacts.

A random number of transformations (between 1 and 6, in a random order) is applied to each image, with the goal of creating a diverse and challenging training set.

## Citation

If you use this dataset in your research, please cite it as follows:

...

## License

...

## Contact

For any questions or issues regarding this dataset, please send a message in the "comments" section of the Kaggle dataset page.

---

Good luck and happy coding! 🚀