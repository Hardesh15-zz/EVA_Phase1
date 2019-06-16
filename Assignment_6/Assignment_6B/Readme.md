## Assignment_6B <br>
### Rewrite model again using these convolutions in the order given below:<br>
  - Normal Convolution<br>
  - Spatially Separable Convolution <br>
  - Depthwise Convolution<br>
  - Grouped Convolution (use 3x3, 5x5 only)<br>
  - Grouped Convolution (use 3x3 only, one with dilation = 1, and another with dilation = 2)<br> 
  - You must use all of the 5 above at least once<br>
  - Train this new model for 50 epochs.<br>
  - Save File as Assignment 6B<br>
## Observation <br>
### Normal Convolution:<br>
Case-1: Only used Convolution and MaxPooling (epochs-50)<br>
Model Accuracy- Not more than 75% <br>

Case-2: Used Batch Normalization and Dropout(only after MaxPooling)(epochs-50)<br>
Model Accuracy- Not more than 79%<br>

Case-3: Used Dropout after each BN but not after MaxPooling<br>
Model Accuracy- Below 80%<br>

Case-4: Used L2 and LR<br>
Model Accuracy- 81.10%(max)<br>

Case-5: Used BN, Dropout, LR, L2, ImageNormalization<br>
Model Accuracy- 82.15%(max)<br>
### Spatially Seperable Convolution<br>
Model Accuracy : 72.01%  <br>
### Depthwise Convolution<br>
Model Accuracy : 81.06%(max)<br>
### Group Convolution with 3x3,5x5 only<br>
Model accuracy - 77.77%(Max)<br>
### Group Convolution (3x3 with D=1 and D=2)<br>
Model Accuracy- 79.92% (Max)<br>
