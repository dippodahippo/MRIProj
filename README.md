# MRIProj
**_A CNN/VGG-19 model trained to detect brain tumors and classify them into 4 categories of brain tumors._** 


The dataset used is kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset and contains **7000+ images for training, testing and validatio**n (655 and 656 for testing and validation respectively.)

Two models were made in this file- **a plain CNN model** and another model transferred over the default **imagenet weights of VGG-19.**
The CNN model has **10 Convolutional Layers**, each sequentially increasing from 64 layers to 512 layers, followed by 4 Dense and Dropout layers going back from 512 to 4 units. The model performs well, providing a **99.96%** **accuracy** overall post training, and a **validation accuracy** of **98.67%.**


Here are the ROC curves and Confusion matrix for the above model-
![image](https://github.com/user-attachments/assets/aaa1bca3-11b1-4329-994d-fc4f34bbabf7)

![image](https://github.com/user-attachments/assets/5e4f6548-94bf-4dd3-899e-86c034de1e1d)


The **VGG-19 Model** takes the default weights from imagenet (I would not generally recommend transferring to the default weights without making the old model trainable, but this was an attempt at transfer learning) and post training, provides an accuracy of **96.45%** and a validation accuracy of **82.47%** towards the end.

And here are the ROC curves and confusion matrix for the VGG-19 model (comparatively terrible, but here they are- )
![image](https://github.com/user-attachments/assets/582192f7-2070-4b9d-8672-c5cca173b4a4)

![image](https://github.com/user-attachments/assets/a01cf35b-db97-4e9b-b9d1-7a18dfeabe90)
