# 4. Keras MLP MNIST Classification
[Notebook](https://colab.research.google.com/drive/1JtWWbSjmaa7uQg1bRoDRPTpMVNdJCYEG)<br>
[Video](https://www.youtube.com/watch?v=jsm6x_UkxCc)<br>

# Quiz
1. Which multi-class classification loss function should be used when:<br>
   - Target labels are one-hot encoded.
   - Target labels are Integer encoded.
- [x] CategoricalCrossentropy for one-hot encoded targets and SparseCategoricalCrossentropy for Integer encoded targets.
- [ ] Both can be used.
- [ ] SparseCategoricalCrossentropy for one-hot encoded targets, CategoricalCrossentropy for Integer encoded targets.
- [ ] BinaryCrossEntropy for one-hot encoded targets and SparseCategoricalCrossentropy for Integer encoded targets.

2. What is the purpose of the method “to_categorical(...)”?
- [x] Convert target class IDs to one-hot encoded vectors.
- [ ] Convert Class labels to Class IDs.
- [ ] Convert one-hot encoded targets to class IDs.
- [ ] None of the above.

3. The softmax activation function is applied in the output layer of a multi-class classification model. Then to calculate model accuracy, the `.argmax(...)` method is applied on the model outputs to find the index of the node with the highest score.<br>
Is applying softmax operation necessary to calculate model accuracy?
- [x] Yes
- [ ] No

4. The cross-entropy (CE) function is defined as following: $\sum_{i=1}^n (y_{i} * log(\hat{y}_{i}))$ Where “n” is the number of classes.<br>
Suppose we have 4 classes. Select the correct CE equation when the prediction vector $\hat{y} = [0.25, 0.3, 0.35, 0.07, 0.03]$ and the target vector is $y = [0.0, 1.0, 0.0, 0.0, 0.0]$?
*This question has multiple correct options and uses partial marking scheme for grading.*
- [x] $-(0.0 * log(0.25) + 1.0 * log(0.3) + 0.0 * log(0.35) + 0.0 * log(0.07) + 0.0 * log(0.07))$
- [ ] $-(0.0 * log(0.25) + 1.0 * log(0.3) + 1.0 * log(0.35) + 0.0 * log(0.07) + 0.0 * log(0.07))$
- [ ] $-(0.0 * log(0.25) + 1.0 * log(0.35) + 1.0 * log(0.30) + 0.0 * log(0.07) + 0.0 * log(0.07))$
- [x] $-(1.0 * log(0.3))$

5. Suppose we are performing a classification task and have 10 input features, we create a network consisting of 3 hidden layers with 3, 5, 4 number of neurons respectively and we have 5 output nodes.
How many layers are present in this network?
- [ ] 5
- [x] 4
- [ ] 3
- [ ] None of the above 