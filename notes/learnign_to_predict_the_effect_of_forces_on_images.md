# Given a force vector applied a certain location in the image authors are tryinng to find the sequential events following that event
# we design a deep neural network model that learns long term sequential dependencies of object movements
while taking into account the geometry and appearance of the scence by combining CNN and RNN

Understand interaction between forces and objects and ability to predict movements caused by the force.

to make an interchangeable dataset.

CNN to encode scene and object appearance and geometry: Image tower
CNN to capture force information: Force tower
RNN that recieves output of 2 CNN and generates object notion or equivalently, a sequence of vectors that represent the velocity of the object at each time. 

Input to force tower to RGB image that represents the impact point, direction and magnitude the query force. 

Ouput of the FC7 layer force tower is provides better results compared to adding the force as another input channel to the real images.

Network is not bale to capture the information in the force image when we havea  single tower for both real images and force images. 


RNN recieves I as input and generates sequecen of velocity vectors. 
The advantage of using RNN is two fold. First, the velocities at different time steps are dependent on each other. the RNN capture these temporal dependecies. 

 
