# 1. Getting started with neural network
[Video](https://www.youtube.com/watch?v=_5XYLA2HLmo&t=15s)<br>
## Quiz
1. An image classification neural network returns an array of numeric values as output.
- [x] True
- [ ] False

2. State whether the following statement is True or False: "A grayscale image is a binary image."
- [ ] True
- [x] False

3. Suppose you have an RGB image of shape (224, 224, 3) and a neural network that only takes grayscale images of size (300, 300, 1) as input. In this scenario, which of the following preprocessing operations are valid?
- [ ] Only resize operation is needed.
- [ ] Apply image cropping with the grayscaling operation.
- [x] Perform resizing and grayscaling operations.
- [ ] Resize the image and pass each channel individually to the network.

4. What do the "knobs" of a neural network model signify?<br>
*This question has multiple correct options and uses partial marking scheme for grading.*
- [x] Tunable parameters of the model.
- [ ] Prediction loss of the model.
- [ ] Input preprocessing operation.
- [x] Weights of the model.

4. What happens to the values of learnable parameters of a model during the training process?
- [ ] Their values remain the same.
- [ ] Their values are initialized again for each set of inputs and outputs.
- [x] Their values are continuously updated as the training progresses.
- [ ] None of the above. 