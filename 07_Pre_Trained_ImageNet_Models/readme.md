# 7. Pre Trained ImageNet Models
[Notebook](https://colab.research.google.com/drive/1KDGfFuzILqP8-9UshN6OJ2iNWbMt5eUW)<br>
[Video](https://www.youtube.com/watch?v=VIYnV5zXals)<br>

## Quiz
1. Which popular deep learning architecture won the ILSVRC in 2012 and significantly improved the state of the art error margin?
- [ ] VGG-16
- [ ] Inception (GoogLeNet)
- [ ] ResNet
- [x] AlexNet

2. Select the correct order for performing image classification using pre-trained models.

    1. Apply model-specific preprocessing function to the input image.
    2. Generate predictions using the .predict(...) method.
    3. Select and load a pre-trained model.
    4. Decode model predictions to get the predicted class label.

- [ ] c → b → a → d
- [x] c → a → b → d
- [ ] a → c → b → d
- [ ] b → a → c → d

3. How many classes can a model trained on the ImageNet dataset predict in TensorFlow?
- [x] 1000
- [ ] 10
- [ ] 100
- [ ] 21000

4. Is preprocessing inputs necessary when using a pre-trained model?
- [x] Yes – Because these models were trained and are used to seeing certain image pixel distributions as inputs during training and the weights have been adjusted accordingly. So to ensure that the model predictions are not wrong due to wrong input pixel distribution, model-specific preprocessing functions should be applied to the input images.
- [ ] No – the model doesn’t return any error, meaning there shouldn’t be any problem with the predictions. 

5. The tf.keras.applications.vgg16.preprocess_input(...) function is responsible for resizing the image and adding the batch dimension to create a 4-d input tensor.
- [ ] True
- [x] False 