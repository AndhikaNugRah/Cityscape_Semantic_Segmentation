# Cityscape_Semantic_Segmentation Used for Self-Driving Car
Semantic Segmentation Experiment Results (Cityscape Dataset):
Semantic segmentation allows vehicles to better understand their environment by identifying different objects on the street. At the same time, instance segmentation identifies each object instance to provide greater depth for calculating speed and distance.

# 1. Network Architectures:

VGG and ResNet: These are Convolutional Neural Network (CNN) architectures commonly used for image classification. They achieve high accuracy by stacking many convolutional layers to extract complex features from images.

FCN (Fully Convolutional Network): This architecture builds upon VGG or ResNet by modifying the final layers to produce pixel-wise predictions for semantic segmentation tasks.

U-Net: This network is specifically designed for semantic segmentation. It has a contracting path (encoder) to capture image features and an expanding path (decoder) to localize and segment objects. It utilizes skip connections between the encoder and decoder to preserve spatial information for accurate segmentation.

# 2. Experiment Data:

Experiment	Dice Loss
1. FCN 8S_Resnet (Epoch 10)	0.3398
2. FCN 8S_Resnet (Epoch 120)	0.3398
3. FCN 8S_Resnet (Epoch 240)	0.2597
4. FCN 8S_VGG (Epoch 160)	0.2892
5. FCN 8S_VGG (Epoch 320)	0.2892
6. Unet (Epoch 320)		0.2483
7. Unet (Epoch 480)		0.2449

# 3. Conclusion:

The experiment results show that the U-Net model achieved the best performance for semantic segmentation based on Dice Loss. The Unet trained for 480 epochs (Experiment 7) achieved the lowest Dice Loss (0.2449) compared to all other models. 

This indicates that U-Net's architecture specifically designed for segmentation tasks outperformed repurposed classification models (FCN) with either VGG or ResNet backbones. Additionally, training U-Net for a longer duration (480 epochs) further improved its performance.

# Dataset Link : https://drive.google.com/drive/folders/1QOUU7tM0SfKr61KkLL9DTBP_Jz5JMOGk?usp=sharing
