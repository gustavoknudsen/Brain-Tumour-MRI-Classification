# Brain Tumor Classification Analysis NN vs. CNN

## Overview
- Investigation Comparing the Results of a Traditional Neural Network vs. a Convolutional Neural Network in Image Classification Tasks.
- Brain Tumor MRI Dataset by Masoud Nickparvar: [[Dataset](https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset)]

## Key Findings
- Validation Accuracy: 94.4% vs. 67.8%
- Model Architecture: Custom CNN (inspired by VGG)
- Classes: Glioma, Meningioma, No Tumor, Pituitary

## Visualizations
- Training/Validation Curves
- Sample Classifications
- Confusion Matrix
- Sample Activation Steps

## Discussion
The investigation clearly showed the power of CNNs when it comes to impage processing. The
CNN massively outperforms the NN in terms of accuracy, precision, recall and F1-scores across
all 4 classes. For the NN, it had some higher values for the recall for ‘notumor’ and ‘pituitary’
which indicates that those are easier to identify. The CNN, for example, has very strong recall
for the ‘notumor’ class, showing near perfect identification.
The NN model struggles to identify all the actual positive cases, despite having a high precision.
The lower recall values show that the model is precise but misses many true cases. The CNN
maintains a good balance between recall and precision.
The large difference between training and validation scores for the CNN suggests that there is
overfitting, especially with the near perfect scores in the training set. However, the validation
scores are still high, showing that, despite overfitting, the parameters generalise well with the
dataset.

## Further Improvements
To improve the model, heavier regularisation should be implemented or the model should be
simplified to address the overfitting. However, 94% accuracy is still a good result and the
investigation clearly showed the benefits of CNNs for image processing and image classification
tasks.
To improve, the architecture of CNN has to be changed. Methods like hyperparameter tuning,
stronger data augmentation and stricter regularisation could help it generalise better with the
dataset. The model was made and not much was changed due to its long training time.
Changing parameters and structure would most certainly improve the performance. By
simplifying the model as well, the training time should be reduced, especially if a convolutional
layer is removed or if the convolutional filters are reduced.
Another option could be to import a pre-trained model, and perform transfer learning on the
dataset. Both of these options would help improve the validation score of the model.

## Setup
1. Clone repository
2. Install requirements
3. Run Jupyter Notebook

## CNN Sample
![image](https://github.com/user-attachments/assets/4ffe135f-0772-4d7f-ab8e-b3bbda738f12)

