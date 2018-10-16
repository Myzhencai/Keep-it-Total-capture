# Keep-it-Total-capture
This repo provide a way to get the same result of Total Capture: A 3D Deformation Model for Tracking Faces, Hands, and Bodies(http://www.cs.cmu.edu/~hanbyulj/totalcapture/)

# Head
For head we use the  monocular camera to get the 3D keypoints of face (https://github.com/Myzhencai/2D-and-3D-face-alignment) , to make the 3D keypoints to the headmesh we used the model (http://flame.is.tue.mpg.de/). By the way , you need to register for the model.
<p align="center"><img src="doc/github_teaser.gif" align="center" width=480 height=auto/></p>

# Hand
For hand we use the special designed monocular cameras to get right and left hand 3D positions of every keypoint .Thanks for Franziska Mueller (https://people.mpi-inf.mpg.de/%7Efrmueller/) share the code for getting the key points . You sir/madam can get the model by applying here (https://handtracker.mpi-inf.mpg.de/projects/GANeratedHands/) ,sending email to her . By the way , please follow the license of the project：GANerated Hands for Real-Time 3D Hand Tracking from Monocular RGB .

# Body
For body we use the monocular camera to get the whole body picture then we use the deeplearning to get the 91 keypoints to get the shape of the whole body . The body model comes from the project : http://files.is.tuebingen.mpg.de/classner/up/ .

# Keep-it-Total-capture model
We modified the model of mano+hand (http://mano.is.tue.mpg.de/) by stiching (replacing) the head (http://flame.is.tue.mpg.de/) of it.
Making the model omnipotence .

# Transferring
For transferring the identity of body , head and hands we used the Deformation-transfer & sdt algorithms .For more details , the paper and code for this project is coming soon. 
