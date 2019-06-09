## Assignment_6
1.Run [this network](https://colab.research.google.com/drive/1STOg33u7haqSptyjUL40FZIxNW4XdBQK)<br> 
After training the network, whatever accuracy you get is your base accuracy. Epochs = 100<br>
### Observation: Model Base Accuracy (After 100 epochs)= 91.52% 
### Validation Accuracy = 82.76% (Max: 83.64%)

2.Fix the network above:<br>
  - remove dense<br>
  - add layers required to reach RF<br>
  - fix kernel scaleup and down (1x1)<br>
  - see if all dropouts are properly placed<br>
  - follow the guidelines we discussed in the class (
  - Get accuracy more than the base accuracy in less number 100 epochs. Hint, you might want to use "border_mode='same',"<br>
  - Save File as Assignment 6A<br>
### Observation: Model validation accuracy (75 epochs) : 84.55% (Max: 85.24%) 
  
3.Rewrite it again using these convolutions in the order given below:<br>
  - Normal Convolution<br>
  - Separable Convolution <br>
  - Depthwise Convolution<br>
  - Grouped Convolution (use 3x3, 5x5 only)<br>
  - Grouped Convolution (use 3x3 only, one with dilation = 1, and another with dilation = 2)<br> 
  - You must use all of the 5 above at least once<br>
  - Train this new model for 50 epochs.<br>
  - Save File as Assignment 6B<br>
Total Score of 600. 400 for Code (300+100), and 200 for documentation (100+100)<br>
Upload the github folder link which has both the files.<br>
