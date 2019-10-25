Machine Learning CS 6375 Project
On Deep Dark Light.


The Folder has 3 files:
accuracy_metrics.py - To calculate the PSNR and SSIM of the output image vs the real image.
test_Dark_Images.py - To test the model on testing dataset.
train_Dark_Images.py - To train the model on training dataset.

Dataset can be downloaded from the link : 
Trained Model can be downloaded from: 
The output images and intermediate Images can be viewed at this link:

Install the required Libraries by using the python pip command.
Library required:
os
scipy.io
tensorflow
tensorflow.contrib.layers
tensorflow.contrib.slim
numpy
rawpy
glob
PIL
skimage.io
skimage.measure
math
cv2

How to Run and Compile:
1. Download the folder and extract it to Dekstop.
2. Download the dataset from the link provided. (Extract it in the same format and keep it inside the Canon folder only)
3. Start the terminal instance on the folder.
4. Start the training of the model by running the command: python train_Dark_Images.py
The model will be trained and will be available at the checkpoint folder. (Our pretrained model can also be downloaded from the link provided above)
5. Start the model test and prediction by running the command: python train_Dark_Images.py
Output will be generated in 4 different folders as Dark Image(Raw Input image scaled with white balance), Scaled Image(Intermediate Output), Output Image(The predicted image from the model), Groundtruth Image(Real Image or expected output)
6. Test the model and accuracy metrics by running the command: python accuracy_metrics.py


References
1.	C. Chen, Qifeng Chen, Jia Xu, and Vladelen Koltun, Learning to see in the dark. CVPR, 2018
2.	Y.Chen and T.pock. Trainable nonlinear reaction diffusion: A flexible framework for fast and effective image restoration. IEEE Transactions on Pattern Analysis and Machine Learning, 39(6),2017.2
3.	K.Dabov, A.Foi, V.Katkovnik, and K.Egiazarian. Image denoising by sparse 3-D transform-domain collaborative filtering. IEEE Transactions on Image Processing,16(8),2007.2,5
4.	X.Dong, G.Wang,Y.Pang,W.Li,J.Wen,W.Meng, and Y.Lu. Fast efficient algorithm for enhancement of lightning video. In IEEE International Conference on Multimedia and Expo, 2011.2
