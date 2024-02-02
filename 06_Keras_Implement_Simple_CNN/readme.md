# 6. Keras Implement Simple CNN
[Notebook](https://colab.research.google.com/drive/1g44ph-zvQM2wQ-kyMeLNAD0o73aX1wHN)<br>
[Video](https://www.youtube.com/watch?v=nYFybn7GXp8)<br>

## Quiz
1. Dropout can be used along with L1 and L2 regularization techniques to prevent the model from overfitting on the training set.
- [x] True
- [ ] False

2. model = tf.keras.Sequential()<br>
model.add(Conv2D(64, kernel_size=5, padding='valid', activation='relu'))<br>
model.add(Conv2D(32, kernel_size=3, padding='same', activation='relu'))<br>
model.add(MaxPooling2D(pool_size=(2, 2)))<br><br>
What is the shape of the output tensor when an tensor of shape of (2, 15, 15, 3) is passed as input to the model above?
- [x] (2, 5, 5, 32)
- [ ] (2, 4, 4, 32)
- [ ] (2, 6, 6, 32)
- [ ] (2, 5, 5, 64) 

    **Explanations:**<br>
    - (2, 15, 15, 3) &rarr; 2 picture of 15px height 15px width, 3 channels RGB color<br>
    - At the output of the first neuron layer &rarr; (2,11,11,64) Because it is possible to translate the kernel by 11 indexes, giving an output matrix of 11x11. With a 5x5 kernel, we lose 4 rows and 4 columns.
    - At the output of the second neuron layer &rarr; (2,9,9,32) Because it is possible to translate the kernel by 9 indexes, giving an output matrix of 9x9. With a 3x3 kernel, we lose 2 rows and 2 columns.
    - At the output of the **MaxPooling2D** &rarr; (2,5,5,32) Because max pooling is performed on a 2x2 pixel window at each step. This reduces the spatial resolution of the feature map by half.

3. The behaviour of the Dropout layer is different during training and inference stage?
- [x] True
- [ ] False

4. Which of the following methods can be used to save model architecture + weights in TensorFlow<br>
*This question has multiple correct options and uses partial marking scheme for grading.*
- [ ] model.compile(...)
- [x] tf.keras.saving.save_model(...)
- [ ] model.save_weights(...)
- [ ] model.summary()
- [x] model.save(...)

5. We can avoid reducing the shape of the output feature map:
*This question has multiple correct options and uses partial marking scheme for grading.*
- [x] By applying padding.
- [x] By using kernels of width and height of 1.
- [ ] By applying strides of size greater than 1 in the convolution operation.
- [ ] By using Max-pooling operation. 