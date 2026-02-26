#### Building Rooftop Extraction from High-Resolution Aerial Images



This project implements a convolutional neural network (CNN) for semantic segmentation of building rooftops from high-resolution aerial imagery.



The objective is to classify each pixel as either rooftop or background using a supervised deep learning approach.



###### \_Data Preparation



Aerial images and corresponding rooftop labels were generated using QGIS and stored locally.

The processed images and labels were then uploaded to the Kaggle environment for GPU-based model training.



Preprocessing steps included:



-Tile generation



-Dataset filtering



-Label correction



-Structuring data for binary segmentation



###### \_Model Architecture



The model follows an encoder–decoder CNN structure:



-Convolutional layers with ReLU activation



-Max pooling for spatial reduction



-Transposed convolution for upsampling



-Softmax output layer



-Binary cross-entropy loss



-Adam optimizer



Two training configurations were evaluated:



-10 epochs



-50 epochs



###### \_Training Environment



Model training was conducted in Google Colab with high-end GPU acceleration settings.



###### \_Repository Structure



bigdata\_final.ipynb        # Model training

test2.ipynb                # Evaluation and visualization

Building\_rooftop\_extraction\_from\_high\_resolution\_Aerial\_images\_Athens.pdf

README.md



###### \_Results



Longer training improved segmentation completeness and boundary refinement.

Limitations remain due to RGB-only imagery, particularly confusion between rooftops and spectrally similar surfaces such as roads.

