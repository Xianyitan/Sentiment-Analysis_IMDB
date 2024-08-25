# LSTM Model for Sentiment Analysis on IMDB Dataset

## Overview
This project implements an LSTM (Long Short-Term Memory) neural network to perform sentiment analysis on the IMDB movie review dataset. The goal is to classify reviews as either positive or negative based on their content. The model is trained on a subset of the dataset and evaluated on a separate test set.

## Model Architecture
The model uses the following architecture:
- **Embedding Layer:** Converts the words in the reviews to dense vectors of fixed size by using pre-trained embedding text file whihc is download from GloVe.
- **LSTM Layer:** This project uses bidirectional LSTM layer to make sure model understand deeply on the training data.
- **Output Layer:** A single neuron with a sigmoid activation function to output a probability score for the binary classification.


### Model Accuracy (Train vs. Test)
![Model Accuracy](./Accuracy%20train%20and%20test%20data.png)
- The training accuracy is slightly higher than the test accuracy, which suggests that the model generalizes well but has some room for improvement.

### Model Loss (Train vs. Test)
![Model Loss](./Loss%20train%20and%20test%20data.png)
- The loss decreases consistently during training, indicating that the model is learning effectively.
- The test loss closely follows the training loss, which suggests that the model is not overfitting significantly.

## Conclusion
The LSTM model demonstrates strong performance on the IMDB sentiment analysis task, with both the accuracy and loss metrics indicating effective learning and generalization. The slight gap between training and test accuracy suggests the potential for further fine-tuning to improve generalization.

## Future Works
- **Data Augmentation:** Explore methods to increase the diversity of the training data, which might improve model generalization.
- **Model Complexity:** Experiment with different model architectures (e.g., deeper LSTM layers, CNNs) to potentially improve performance.
