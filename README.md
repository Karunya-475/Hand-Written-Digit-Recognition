# Handwritten Digit Recognition

**Decoding human handwriting into machine-readable intelligence.**

An end-to-end computer vision pipeline using Deep Learning and the MNIST dataset to classify handwritten digits ($0–9$) with high accuracy and full reproducibility.

---

###  Introduction
Handwritten digit recognition bridges visual input and numerical data. Using the standard **MNIST dataset** ($70,000$ grayscale $28 \times 28$ images), this project builds a model trained on $60,000$ samples and evaluated on $10,000$ test images to deliver fast, reliable digit predictions.

###  Data Processing Class Distribution: 

* Confirmed balanced target classes (~ 5,400 to 6,700 samples per digit) to eliminate model bias.  

* Normalization: Rescaled raw pixel intensities from [0, 255] to [0.0, 1.0] for faster convergence.  

* Reshaping: Flattened 28 X 28 matrix inputs into 784-element vectors for sequential feedforward layers.

###  Model Explanation Architecture: 

* Sequential neural network utilizing an Input/Flatten layer, hidden Dense layers with ReLU non-linearity, and a 10-node Softmax output layer for multi-class probabilities.

* Compilation: Trained using the Adam optimizer and sparse_categorical_crossentropy loss tracking accuracy across training and test splits.

 ###  Conclusion: 
 
* Established a benchmark pipeline for digit classification with complete run-to-run reproducibility.

* Next Steps: Extend architecture to Convolutional Neural Networks (CNNs) and deploy via a Streamlit web app for real-time canvas predictions.
