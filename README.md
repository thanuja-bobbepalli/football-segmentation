# Football Image Segmentation

##  Project Overview
This project focuses on semantic segmentation of football images using deep learning. The model is trained to segment different objects in football scenes, such as players, the ball, and the field. The implementation is done in **PyTorch**, and the dataset used is from **Kaggle**.

### Dataset Information
Dataset link : **[Football Semantic Segmentation Dataset](https://www.kaggle.com/datasets/sadhliroomyprime/football-semantic-segmentation)**

### **Dataset Description**
This dataset consists of 300 image files :

- Original Images:100 
    
- Mask Images    :100
    
- Saved Image    :100

 Total image pairs used :100
 
  --> 80 pairs used for training
  
  --> 10 pairs used for validation
  
  --> 10 pairs used for testing 

### Models Used:
- **U-Net**
- **Transformed U-Net**
- **Attention U-Net**
- **U-Net with ResNet-50 Backbone**
- **U-Net with ResNet101 Backbone**

###  Loss Function Used 
- Hybrid Loss(Dice + Focal Loss  ) 

### **Performance Metrics**
The model is evaluated using:
- **Dice Coefficient**: Measures segmentation accuracy
- **Loss Curves**: Training vs Validation loss plots

### **Results** 
###### For initial learning rate 0.001 & 0.005 
----
                Baseline Unet  |   Transformed Unet | Attention Unet | ResNet 50  |  ResNet101
   
    Test Loss    	0.2204             0.2268               0.2512        0.2274        0.2300
    Test Dice Score   0.7432             0.6297               0.5806        0.6495        0.5955

----

### Conclusion 
This project compares different deep learning models for football image segmentation using 100 image pairs across 11 classes. Five models—Baseline U-Net, Transformed U-Net, Attention U-Net, ResNet-50 U-Net, and ResNet-101 U-Net—were tested and optimized using a hybrid loss function (Dice + Cross-Entropy)

The Baseline U-Net performed the best, achieving the highest accuracy and lowest loss, while more complex models like ResNet-based U-Nets and Attention U-Net did not show significant improvement. This suggests that for football segmentation, a well-optimized U-Net can be more effective than deeper architectures.

Despite the small dataset, the loss was successfully reduced to 0.19–0.2, demonstrating that careful model selection and loss function tuning can lead to strong results. Future improvements could include better data augmentation, different backbone networks, and post-processing techniques to refine segmentation accuracy.


     


 


