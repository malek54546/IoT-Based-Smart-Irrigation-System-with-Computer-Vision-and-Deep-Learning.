# IoT-Based Smart Irrigation System with Computer Vision and Deep-Learning.

###############################################################################

# ABSTRACT 
This project introduces a Smart Irrigation System that combines IoT and AI technologies to 
optimize water use and improve crop productivity.   
The system monitors soil moisture, temperature, and humidity, and automatically controls 
irrigation based on real time data. Users can manage the system remotely via a mobile app, while 
key data are displayed on an LCD screen.  
A high-resolution camera uses AI to monitor plant health and detect diseases. Powered by 
a rechargeable battery, the system is practical, energy-efficient, and reduces manual labor. This 
solution promotes sustainable agriculture by minimizing water waste and enabling precise, 
automated irrigation.




Plant Health Monitoring via MobileNetV2: the disease detection module, we implemented a Deep Learning model based on the MobileNetV2 architecture. This choice was driven by the need for an efficient, lightweight model capable of performing real-time diagnosis on edge computing devices (Raspberry Pi).

• Model Architecture: MobileNetV2 utilizes "Depthwise Separable Convolutions" which significantly reduces the number of parameters and computational complexity without sacrificing high accuracy.

• Dataset & Training: The model was trained on a specialized dataset containing images of Apple and Grape leaves, covering various pathologies like Apple Scab and Black Rot.

• Training Parameters:

o Image Input: Resized to 224x224 pixels.

o Epochs: 13 (reaching convergence with high stability).

o Optimization: Adam Optimizer with a learning rate of 0.0001 and Dropout (0.2) to prevent overfitting.

o Val_accuracy : 96.2 %

###############################################################################

#Training...

Epoch 1/13
Epoch 1: val accuracy improved from -inf to 0.88587, saving model to C:\Users\malek\Desktop\msf\G_A_mlnet.h5
140/14049s loss: 1.2121 accuracy: 0.5730 val loss: 0.3832 val accuracy: 0.8859 Ir: 0.0010 49s/epoch- 347ms/step Epoch 2/13

Epoch 2: val accuracy improved from 8.88587 to 0.92572, saving model to C:\Users\malek\Desktop\msf\G_A_mlnet.hs
148/140495 loss: 0.6171 accuracy: 0.7834 val loss: 0.2628 val accuracy: 0.9257 1r: 0.0010 49s/epoch 348ms/step Epoch 3/13

Epoch 3: val accuracy improved from 0.92572 to 0.93841, saving model to C:\Users\malek\Desktop\msf\G_A_mInet.h5
140/140475 loss: 0.4955 accuracy: 8.8211val loss: 0.1912 val accuracy: 0.9384 Ir: 0.0010 47s/epoch- 333ms/step Epoch 4/13

Epoch 4: val accuracy improved from 0.93841 to 0.94565, saving model to C:\Users\malek\Desktop\msf\G_A_mlnet.h5
140/14047s loss: 0.4333 accuracy: 0.8458 val loss: 0.1756 Epoch 5/13 val accuracy: 0.9457 Ir: 0.0010 47s/epoch- 335ms/step

Epoch 5: val accuracy did not improve from 0.94565
148/140465 loss: 0.3633 accuracy: 0.8679 val loss: 0.1707 val accuracy: 0.9438 1г: 0.0010 46s/epoch 330ms/step Epoch 6/13

Epoch 6: val accuracy improved from 0.94565 to 0.94746, saving model to C:\Users\malek\Desktop\msf\G_A_minet.hs
140/148465 loss: 0.3578 accuracy: 0.8719 val loss: 0.1697 val accuracy: 0.9475 Ir: 0.001046s/epoch 331ms/step Epoch 7/13

Epoch 7: val accuracy improved from 0.94746 to 8.96196, saving model to C:\Users\malek\Desktop\msF\G_A_mlnet.h5
140/140 50s loss: 0.3309 accuracy: 0.8827 val loss: 0.1243 val accuracy: 0.9620 Ir: 0.0010 50s/epoch 354ms/step
Epoch 8: val accuracy did not improve from 0.96196
140/14054s loss: 0.3019 accuracy: 0.8890 val_loss: 0.1438 val accuracy: 0.9565 1r: 0.001054s/epoch- 383ms/step Epoch 9/13

Epoch 9: val accuracy did not improve from 0.96196
Epoch 9: ReduceLROnPlateau reducing learning rate to 0.0005000000237487257.
140/14053s loss: 0.2764 accuracy: 0.9056 val_loss: 0.1324 val_accuracy: 0.9583 Ir: 0.001053s/epoch- 377ms/step Epoch 10/13

Epoch 10: val accuracy did not improve from 0.96196
Restoring model weights from the end of the best epoch: 7.
140/14049s loss: 0.2512 accuracy: 0.9133 val_loss: 0.1168 val_accuracy: 0.9620 1r: 5.0000e-04 49s/epoch - 351ms/step 
Epoch 10: early stopping.

##################################################################################

#Sample Plant Images and Classification Results: 

https://drive.google.com/drive/folders/13Pvsk8UNOjJi7EyT-d-oNDM6-HNlCKIG?usp=sharing





















