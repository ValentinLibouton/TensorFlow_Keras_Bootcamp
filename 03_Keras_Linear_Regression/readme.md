# 3. Keras Linear Regression
[Notebook](https://colab.research.google.com/drive/1cnABAGOvvd6p6tBmwiXggoHyWKDqQmFu)<br>
[Video](https://www.youtube.com/watch?v=yuAZQJ5BnJk)<br>

## Quiz
1. Regression is a supervised learning technique that aims to model the relationship between one or more input variables (features) and a continuous (target) variable.
- [x] True
- [ ] False

2. A linear regression model can fit a non-linear relationship between one or more input variables (features) and a continuous (target) variable. This is possible because we use a weighted sum of features to express their relationship with the target variable.
- [ ] True
- [x] False

3. Suppose we have a regression dataset containing 11 features. What is the total number of training parameters of the model in scenarios:<br>

   - When we use 10 of the features with bias.<br>
   - When we use 5 features without bias.<br>
- [x] 11 and 5
- [ ] 10 and 5
- [ ] 11 and 6
- [ ] 20 and 6

4. What is the purpose of executing the "model.compile(...)" operation?<br>
*This question has multiple correct options and uses partial marking scheme for grading.*
- [x] Specify the loss function to use.
- [ ] To train the model.
- [ ] Initializing model parameters.
- [x] Selecting the optimizer and setting a learning rate.
- [x] Specify metrics to be used for evaluating model performance.

5. Which method in Tensorflow is used to generates model predictions?
- [ ] model.fit(...)
- [ ] model.evaluate(...)
- [ ] model.compile(...)
- [x] model.predict(...)
- [ ] model.summary(...) 