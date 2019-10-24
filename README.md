# Eye_tracking

## Dataset
CNN Model is trained with processed MPIIGAZE dataset. 

## Image processing
Image processing is conducted by OpenCV and Dlib.

## CNN Model 
CNN Model has 24 Layers. Each eye image goes through 11 CNN layers, and then goes through two dense layers after being merged into one. 


After building CNN model, I optimized the model using Depthwise Separable Convolution.


After optimizing, model’s test Mean Squared Error increased, but file-size and number of parameters decreased.

This is the model drawing by tensorboard

![11](https://user-images.githubusercontent.com/39719936/67455002-1c65aa80-f667-11e9-98f1-8e813f5b2805.png)

## Result

This is the model's cost(MSE) graph</br>

<img width="500" alt="캡처" src="https://user-images.githubusercontent.com/39719936/67455089-68b0ea80-f667-11e9-8dd0-f4e175848b7c.PNG">



<img width="600" alt="캡처_2" src="https://user-images.githubusercontent.com/39719936/67455290-2dfb8200-f668-11e9-92fd-088d955ea813.PNG">

## Reference

X. Zhang, Y. Sugano. et al. “MPIIGAZE:Appearance-basedGaze Estimation in the Wild.” Proc. of the IEEE Conference on Computer Visionand Pattern Recognition (CVPR), June, p.4511-4520, 2015

Bradski G. The OpenCV Library. Dr Dobb&#39;sJournal of Software Tools.2000

Davis E. King. Dlib-ml: A Machine Learning Toolkit. Journal of Machine LearningResearch 10,pp. 1755-1758, 2009


Howard, Andrew G. et al. “MobileNets: Efficient Convolutional Neural Networksfor Mobile Vision Applications.” ArXiv abs/1704.04861 2017.

François Chollet. “keras”. GitHub, GitHub repository 2015
