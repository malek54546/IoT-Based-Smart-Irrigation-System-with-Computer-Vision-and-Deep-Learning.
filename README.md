# IoT-Based Smart Irrigation System with Computer Vision and Deep-Learning.

###############################################################################

Plant Health Monitoring via MobileNetV2: the disease detection module, we implemented a Deep Learning model based on the MobileNetV2 architecture. This choice was driven by the need for an efficient, lightweight model capable of performing real-time diagnosis on edge computing devices (Raspberry Pi).

• Model Architecture: MobileNetV2 utilizes "Depthwise Separable Convolutions" which significantly reduces the number of parameters and computational complexity without sacrificing high accuracy.

• Dataset & Training: The model was trained on a specialized dataset containing images of Apple and Grape leaves, covering various pathologies like Apple Scab and Black Rot.

• Training Parameters:

o Image Input: Resized to 224x224 pixels.

o Epochs: 13 (reaching convergence with high stability).

o Optimization: Adam Optimizer with a learning rate of 0.0001 and Dropout (0.2) to prevent overfitting.










