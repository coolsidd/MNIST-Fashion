 # MNIST-Fashion

## The Convolutional Neural Net
This implementation of CNN uses stacked layers as used in [the inception network](https://www.cs.unc.edu/~wliu/papers/GoogLeNet.pdf "Going deeper with convolutions"). However it uses a different ratio of stacking and sizes of filters. This implementation also uses [residual layers](https://www.cv-foundation.org/openaccess/content_cvpr_2016/papers/He_Deep_Residual_Learning_CVPR_2016_paper.pdf "Deep Residual Learning") to futher increase accuracy

## Summary of the net

This convolutional neural network contains over 4 million parameters.

Total params: 4,037,002
Trainable params: 4,035,850
Non-trainable params: 1,152


## Data Augmentation and training
The images of the dataset were horizontally flipped and shuffled.
The images were padded and the model was trained on batchnormalized data.

## Results

| Type                            | Number of images | Percentage of Dataset | Accuracy achieved |
|---------------------------------|------------------|-----------------------|-------------------|
| Dev  (unseen)                   | 8000             | 11.43%                | 93.4%             |
| Test (unseen, only tested once) | 2000             | 2.86%                 | 94.2%             |
| Training set                    | 60000            | 85.71%                | 95.5%*            |

The value reported is the average over augmentation
