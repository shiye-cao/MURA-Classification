# MURA
Intersession 2019- Deep Learning for Medical Image Analysis Class Final Project
Experimented with various Pytorch deep learning models including VGG16, DenseNet and Resnet on musculoskeletal radiographs(MURA) dataset provided by Stanford Univeristy School of Medicine. 

# Dataset: 
The MURA (musculoskeletal radiographs) dataset provided by Stanford University School of Medicine consists of 14,863 studies from 12,173 patients, with a total of 40,561 multi-view radiographic images (each manually labeled as normal or abnormal by radiologists from the Stanford Hospital and separated into 7 groups based on the body part: elbow, finger, forearm, hand, humerus, shoulder, and wrist). 

Due to the limited time constraint, I chose to work with only 2 datasets (finger-4708 images and wrist-6974 images). I pre-processed the data by picking out the images that showed more than one x-ray at a time. I also randomly picked out 75 normal images and 75 abnormal images from the MURA dataset to use as the validation dataset. 

# Clinical Significance: 
Today, musculoskeletal conditions affect more than 1.7 billion people worldwide, and are the most common cause of severe, long-term pain and disability, with 30 million emergency department visits annually and increasing. I hope that through deep learning, my model can make diagnosis beyond the level of current expert radiologist. That way, in the future, the model can be used to help radiologist make better judgements on whether an X-ray study is normal or abnormal. 

# Experiments: 
To find the best deep learning model, I experimented with 3 different models including: ResNet18, DenseNet161, and VGG16. I have also experimented with various other factors including: Convolution Neural Net, the number of epochs, and Pre-training. I chose to not test the effects of data augmentation on the dataset since there is enough variation in the dataset with images from all kinds of different view point, although images with more than one X-ray in the frame was taken out of the dataset during pre-processing. 

# Final Model: VGG16 Model without ConvNet and with pre-training and 25 epochs.

# Conclusion: 
The deep learning model performed better than the radiologists on both the wrist and the finger dataset. So, I see a value in generalizing the model to all 7 datasets and together it will likely become a computer radiologist that performs better than the current human radiologists. 

For details regarding this project and my Experimental Results Please See the MURA Report Document.
 
# Citation: 
BSD 3-Clause License

Copyright (c) 2017, Pytorch contributors
All rights reserved.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:

* Redistributions of source code must retain the above copyright notice, this
  list of conditions and the following disclaimer.

* Redistributions in binary form must reproduce the above copyright notice,
  this list of conditions and the following disclaimer in the documentation
  and/or other materials provided with the distribution.

* Neither the name of the copyright holder nor the names of its
  contributors may be used to endorse or promote products derived from
  this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
