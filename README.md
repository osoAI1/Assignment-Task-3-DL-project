
## Human Activity Recognition using CNN-LSTM

 A hybrid deep learning model combining Convolutional Neural Networks (*CNN*) for spatial feature extraction and Long Short-Term Memory (*LSTM*) for temporal sequence modeling is implemented

The name of dataset: Human Activity Recognition (*HAR* - Video Dataset) and the size of it is *14.8G* 
https://www.kaggle.com/datasets/sharjeelmazhar/human-activity-recognition-video-dataset

- Walking: 171 videos
- Sitting: 156 videos
- Standing Still: 174 videos

This project aims to classify video clips into three types or classes(Walking, Sitting, Standing Still) of 7 class(Clapping, Meeting and splitting, Sitting, Standing still, Walking, Walking while reading a book,Walking while using the phone)

All videos are standardized to **10 frames** of size **32×32 pixels** with 3 RGB channels
 **CNN**: Two convolutional layers (Conv2D) followed by MaxPooling and AdaptiveAvgPool2d to extract 64 features per frame
 **LSTM**: One LSTM layer with input size 64 (feature dimension) and hidden size 64
 **Final layer**: Fully Connected layer with 3 output nodes (one per class)
 
<img width="1176" height="405" alt="image" src="https://github.com/user-attachments/assets/5229e44c-0ca0-407c-a74e-15af4f41ab59" />


## Hyperparameters

   -**Epochs**: 30
   -**Batch Size**: 16
   -**learning rate**: 1e-3

**Optimizer**: Adam 

**Loss Function**: CrossEntropyLoss

##
**Test Accuracy: 0.9109**

<img width="581" height="516" alt="image" src="https://github.com/user-attachments/assets/3cb815ba-f2ce-4343-842a-b2e040e535a7" />

<img width="691" height="393" alt="image" src="https://github.com/user-attachments/assets/85a672ea-681f-4429-96d8-249e9b5afd8f" />

<img width="789" height="418" alt="image" src="https://github.com/user-attachments/assets/38be3dc5-370e-4b7b-a22b-74f70169b043" />
