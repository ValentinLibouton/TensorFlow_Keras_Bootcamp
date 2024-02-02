# 2. Fundamentals of Training a Neural Network
[Video](https://www.youtube.com/watch?v=4E2_rkP3owI)<br>

## Notes
If the probabilities are:
```python
{cat:0.37, dog:0.50, other:0.13}
```
SSE:
```latex
\large{\text{SSE} = (1 - 0.37)^2 + (0 - 0.50)^2 + (0 - 0.13)^2 = 0.6638}
```

MSE:
```latex
\large{\text{MSE} = \frac{1}{n}  \sum_{i=1}^{n}(y_{i} - y^{'}_{i})^2 = \text{mean(SSE)} = 0.2213}
```

## Quiz
1. Suppose there are 5 classes in-order: Lion, Tiger, Elephant, Cheetah, and Leopard. Which of the following represents the correct one-hot encoded representation for Elephant and Leopard?
- [ ] [0,0,1,0,0] and [0,0,1,0,1]
- [ ] [1,0,1,0,0] and [0,0,0,0,1]
- [x] [0,0,1,0,0] and [0,0,0,0,1]
- [ ] [0,0,1,0,1] and [0,0,1,0,1]

2. Select the correct **SSE loss equation** for the following prediction vector: $\hat{y} = [0.10, 0.005, 0.40, 0.10, 0.35]$ and target vector: $y = [0,1,0,1,1]$
- [ ] $(0 - 0.10) + (1 - 0.05) + (0 - 0.40) + (1- 0.10) + (1 - 0.35)$
- [x] $(0 - 0.10)^{2} + (1 - 0.05)^{2} + (0 - 0.40)^{2} + (1 - 0.10)^{2} + (1 - 0.35)^{2}$
- [ ] $((0 - 0.10)^{2} + (1 - 0.05)^{2} + (0 - 0.40)^{2} + (1 - 0.10)2 + (1 - 0.35)^{2}) / 5$
- [ ] $(1 - 0.10)^{2} + (0 - 0.05)^{2} + (1 - 0.40)^{2} + (1 - 0.10)^{2} + (0 - 0.35)^{2}$

3. Gradient Descent is used to tune the learning rate hyperparameter.
- [ ] True
- [x] False

4. Which one of the following represents the correct formula to perform weight updates:<br>
*This question has multiple correct options and uses partial marking scheme for grading.*
- [ ] $W_{new} = W_{current} + learning\_rate * gradient$
- [x] $W_{new} += -learning\_rate * gradient$
- [ ] $W_{new} -= -learning\_rate * gradient$
- [x] $W_{new} = W_{current} - learning\_rate * gradient$
- [ ] $W_{new} += -learning\_rate * -gradient$

5. Why should the training set be passed multiple times through the neural network?<br>
*This question has multiple correct options and uses partial marking scheme for grading.*
- [x] Adjust the weights of the network as best as possible.
- [x] To reduce the prediction loss of the model.
- [ ] To find the best learning rate for the model.
- [ ] To reduce the prediction accuracy of the model.
- [x] To improve the model's classification accuracy. 