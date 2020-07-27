# Facial-Recognition-System
Facial Recognition System in PyTorch
  This is a PyTorch implementation of the "FaceNet: A Unified Embedding for Face Recognition and Clustering".
 
  LFW dataset is used for training and testing.
  
# Data Preprocessing
Data is preprocessed by making triplets of training images. Each triplet contains
  1. An Anchor image
  2. A Postive image
  3. A Negative image

Both Anchor and Postive image have same label while a negative has different labael as mentioned in the paper.

# Loss Function
Siamese NN and triplet loss function for Training. The loss function can be described using a Euclidean distance function
  
    L(A, P, N) = max(||f(A) - f(P)||^2 - ||f(A) - f(N)||^2 + alpha, 0)


# Classifier
K Neighrest Neighbour (KNN) is used for Classification.
