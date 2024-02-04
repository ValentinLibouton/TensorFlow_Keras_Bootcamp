# 9. Keras Segmentation TensorFlow Hub
[Notebook](https://colab.research.google.com/drive/1ZXrPGR84wLucDrMko5h7WwfY9Psay6po)<br>
[Video](https://www.youtube.com/watch?v=U4TnGPyoJaw)<br>

## Quiz
1. What is the main objective of semantic segmentation in deep learning?
- [x] Classifying individual pixels in an image into categories.
- [ ] Identifying bounding boxes around objects in an image.
- [ ] Predicting the class label for an entire image.
- [ ] Determining the keypoints of an object in an image. 

2. In a semantic segmentation task, what is typically the output of the deep learning model?
- [ ] A scalar value representing the class label
- [ ] A set of bounding box coordinates
- [x] A pixel-wise probability map
- [ ] A list of keypoints

3. How many classes does the CamVid dataset contain?
- [x] 32
- [ ] 33
- [ ] 31
- [ ] 30

4. What is the primary reason for mapping class IDs to RGB pixels in semantic segmentation?
- [ ] To convert the input image into a grayscale format.
- [ ] To simplify the architecture of the model.
- [x] To visually represent the segmented regions with different colors for better interpretation.
- [ ] To reduce the computational complexity of the model.

5. Which of the following line of code is used to load pre-trained models from TensorFlow-Hub?
- [ ] model = hub.load_model(model_url)
- [ ] model = tf.keras.models.load_model(model_url)
- [x] model = hub.load(model_url)
- [ ] None of the above. 