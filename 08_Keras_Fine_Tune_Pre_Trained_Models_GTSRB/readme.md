# 8. Keras Fine Tune Pre Trained Models GTSRB
[Notebook](https://colab.research.google.com/drive/1iWlBfa0kHEBb0peoF6kKo5yCLXIZkPJw)<br>
[Video](https://www.youtube.com/watch?v=10uDPsdAUdY)<br>
[Docs: Keras &rarr; image data loading](https://keras.io/api/data_loading/image/)

## Quiz
1. What is transfer learning in the context of deep learning?
- [ ] Training a model from scratch for a specific task.
- [x] Using a pre-trained model as a starting point and adapting it to a new task.
- [ ] Combining multiple models to create a single, more powerful model.
- [ ] Implementing a completely new neural network architecture.

2. Which of the following is a common reason to use transfer learning?
- [x] To save computational resources.
- [ ] To increase the complexity of a model.
- [ ] To create a larger dataset for training.
- [ ] To test the robustness of a model.

3. In fine-tuning, what is generally done to the backbone layers of a pre-trained model?
- [ ] They are replaced by new layers.
- [ ] Their weights are initialized randomly
- [x] Some or all weights in the backbone are updated to make the model more robust on the new task.
- [ ] Their weights are removed entirely.

4. In practice, even though we have small amount of data it is highly recommended to create and train models from scratch them rather than using pre-trained models?
- [ ] True - because then you can fully control your model architecture, parameters, and hyperparameters.
- [x] False - we should start with pre-trained models as these models have been trained on massive datasets. The early layers of feature extractors generally learn how to detect low-level features such as points, edges, curves, etc., which can be helpful in various tasks.
- [ ] None of the above.

5. Suppose we have moderate-size data. Do we fine-tune the whole pre-trained model or only train the parameters of the new layer we have added?
- [ ] We should only train layers of the model that are different from the pre-trained model.
- [ ] We should train all layers of the model.
- [ ] We should train the new layers for some epochs and then train the whole model.
- [x] Depending on the task, we might have to experiment and check what works best for our use case.
- [ ] None of them 