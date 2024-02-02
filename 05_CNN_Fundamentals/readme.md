# 5. CNN Fundamentals
[Video](https://www.youtube.com/watch?v=_OkF3w_ZMKE)<br>

## Quiz
1. Choose the correct statements from the following:<br>
*This question has multiple correct options and uses partial marking scheme for grading.*
- [x] MLPs are more prone to overfitting than CNNs.
- [ ] CNNs are more prone to overfitting than MLPs.
- [x] In MLPs, every neuron in a layer is connected to every other neuron in the next layer.
- [x] Parameter sharing is one of the key properties of CNNs that help them to reduce overfitting than MLPs
- [ ] MLPs are translation invariant.

2. What is the value of X after performing a convolution operation when the kernel's center is at position (3, 3) in the input matrix.
   - The 5x5 matrix is the Input and the first 3x3 matrix is the kernel.
   - Assume row and column are 1-indexed.
   $\begin{bmatrix}7& 2& 3 & 3& 8\\4 & 5& 3 & 8& 4\\3 & 3& 2 & 8& 4\\2 & 8& 7 & 2& 7\\5 & 4& 4& 5& 4\\\end{bmatrix}  \,\, *  \begin{bmatrix} 1 & 0 & -1\\ 1 & 0 & -1\\1 & 0 & -1 \end{bmatrix}  \,\, = \begin{bmatrix}  ..& .. & ..\\ .. & X & ..\\ .. & .. & .. \end{bmatrix}$
- [ ] 2
- [ ] 0
- [x] -2
- [ ] 8

3. What happens to the receptive field size of kernels as we go deeper into the model?
- [x] It becomes bigger.
- [ ] It remains the same.
- [ ] The receptive field decreases exponenetially as we go deeper in the network. 

4. In a convolution layer, if the number of channels in the Input matrix is 10, then what should be the number of channels in the kernel matrix?
- [ ] 5
- [x] 10
- [ ] 9
- [ ] 1

5. Choose True or False for the following statements:
   - Max Pooling is used to shrink the size of the feature map.
   - The max pooling operation is the only pooling operation available.
- [x] True, False.
- [ ] True, True
- [ ] False, False 