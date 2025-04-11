# Image Retrieval Based on a Hybrid Model of Deep Convolutional Encoder

This project presents an effective hybrid deep learning model for content-based image retrieval (CBIR), designed to bridge the semantic gap in visual search tasks. The proposed approach integrates a 6-layer Convolutional Neural Network (CNN) with a 3-layer Autoencoder for high-level semantic feature extraction and dimensionality reduction, respectively. The CNN captures rich, abstract visual features, while the autoencoder compresses the 2048-dimensional vectors into compact 128-bit representations.

To enable efficient large-scale retrieval, the compressed features are indexed using Euclidean distance algorithm, facilitating fast query matching via distance based similarity search. The training utilizes the binary cross-entropy loss function, employing optimizers Adam, with Batch Normalization and Dropout incorporated to improve generalization and convergence.


This is our model Architecture which is used - 
![image](https://github.com/user-attachments/assets/84fd9e63-ba3b-4d9f-8936-d7e34b035667)

I trained the model on Animal Dataset, you can get the dataset used by running this code- 

import kagglehub
path = kagglehub.dataset_download("theaayushbajaj/cbir-dataset")
print("Path to dataset files:", path)


After training of model, input image provides to model for test - 

<img width="583" alt="image" src="https://github.com/user-attachments/assets/1fa65555-474a-45ea-aff6-05a23be89367" />

recieved output from model is-

<img width="1222" alt="image" src="https://github.com/user-attachments/assets/313c1682-746a-441d-a74a-645c6545c2f3" />


