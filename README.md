# VGG16_Model_MURA
Implemented a CNN architecture on VGG16 model to determine whether an X-ray study is normal or abnormal.
Musculoskeletal conditions affect more than 1.7 billion people worldwide, and are the most common cause of severe, long-term pain and disability, with 30 million emergency department visits annually and increasing. The dataset can lead to significant advances in medical imaging technologies which can diagnose at the level of experts, towards improving healthcare access in parts of the world where access to skilled radiologists is limited.

MURA is one of the largest public radiographic image datasets. The dataset is made available to the community and hosting a competition to see if your models can perform as well as radiologists on the task.


Reference: https://stanfordmlgroup.github.io/competitions/mura/

In this, I have applied InceptionV3 model to detect abnormality through X-ray images.

Reshaping the images to be of size 512x512 which is the size used in most of the MURA implementaions on github. Reshaping is done by black padding the images so that the original image stays in the center.

Apply image augmentation techniques like : a. Horizontal flipping b. Random rotation upto 30 degrees

Intially, I used pretrained weights on imagenet and then started unfreezing the weights and started training a few layers from last and improved the accuracy

Employed early stopping to avoid overfitting. Apart from that also tried drop out.
