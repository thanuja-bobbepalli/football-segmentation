# Football Image Segmentation

##  Project Overview
This project focuses on semantic segmentation of football images using deep learning. The model is trained to segment different objects in football scenes, such as players, the ball, and the field. The implementation is done in **PyTorch**, and the dataset used is from **Kaggle**.

# 📂 Dataset Information
Dataset link : **[Football Semantic Segmentation Dataset](https://www.kaggle.com/datasets/sadhliroomyprime/football-semantic-segmentation)**

# **Dataset Description**
This dataset consists of 300 image files :

- Original Images:100 
    
- Mask Images    :100
    
- Saved Image    :100

 Total image pairs used :100
 
  --> 80 pairs used for training
  
  --> 10 pairs used for validation
  
  --> 10 pairs used for testing 

# Models Used:
- **U-Net**
- **Transformed U-Net**
- **Attention U-Net**
- **U-Net with ResNet-50 Backbone**
- **U-Net with ResNet101 Backbone**

#  Loss Function Used 
- Hybrid Loss(Dice + Focal Loss  ) 

# **Performance Metrics**
The model is evaluated using:
- **Dice Coefficient**: Measures segmentation accuracy
- **Loss Curves**: Training vs Validation loss plots
# Contributor:
 


