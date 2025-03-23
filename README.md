# M3P04 CNN Bird Classification Project
--------

**Overview:** <br>

The goal of this project is to build an image classification model that can classify bird species from images. The dataset used for this project is the Bird Species dataset from Kaggle, containing images from 20 different bird species. The model will be trained to recognize and classify these bird species, with the objective of achieving at least 85% accuracy on the test set.<br>

Note: This project was done on Google Colab: <br>
- The 'images to predict', 'test', 'train' and 'valid' folders were saved in a new folder called 'Bird_Data' and uploaded into Google Drive.
- The directory paths for the dataset and for prediction were in Google Drive.

**Dataset Details:** <br> 

The dataset consists of images from 20 bird species. It is divided into three subsets for training, validation, and testing: <br>
- Training Set: 3208 images (approximately 160 images per species) <br>
- Validation Set: 100 images (5 images per species) <br>
- Test Set: 100 images (5 images per species) <br>
- Additionally, there is a set of "images to predict" that will be used to evaluate the final performance of the trained model. <br>

**Dataset link:** https://www.kaggle.com/datasets/umairshahpirzada/birds-20-species-image-classification/data
  
**Criteria Checklist:** <br>  
- Model: A pretrained VGG16 (CNN) model was used. Added layers and customized the model for data training and validation. 
- Accuracy: The model was able to achieve an accuracy of at least 85% on the test set.
- Final Evaluation: After training, the images in the "images to predict" folder was used to evaluate the final model's performance. 

**Approach:** <br> 

1. **Data Preprocessing:** <br> 
- Data Augmentation: Data augmentation techniques such as rotations, axis shift, flips etc. were used to make the model more robust and improve generalization.

2. **Model Selection:** <br> 
- A pretrained VGG16 model was used, and additional layers were added to customize the model for data training and validation. This model was used for image classification.

3. **Model Training:** <br>  
- The model was trained using the training set.
- The validation set was used during training to monitor and prevent overfitting.

4. **Evaluation:** <br>
- Evaluation was performed on the model using the test set to ensure that it meets the required accuracy (85%).

5. **Final Model Testing:** <br>
- After training, an image from the "images to predict" folder was used to evaluate the final performance of the model. This will help assess how well the model generalizes to unseen data.

**Conclusion:** <br>
- At Epoch 50, Training accuracy was 85.0686%.
- At Epoch 50, Validation accuracy was 92%.
- After training, Test Accuracy was 91%. (meets criteria of having at least 85%)
- Classification Report Accuracy was 91%.
- Prediction: Using '2.jpg' from 'images to predict' folder, the model predicted the bird species class to be the AFRICAN CROWNED CRANE.
