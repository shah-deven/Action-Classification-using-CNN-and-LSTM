# Action-Classification-using-CNN-and-LSTM

In this project, CNN - LSTM is trained to classify human actions. LSTMs are designed to handle sequential data.
For human action recognition, skeleton data is used that encodes the 3D locations of 25 body joints. The data is collected by Kinect v2. There are 10 different action classes. There are 4000 training sequences, 800 validation sequences, and 1000 test sequences. Each sequence has 15 frames, each frame is a 75-dimension vector (the xyz positions of 25 joints).

The following extra packages are required to run this:
pip install h5py
pip install git+https://github.com/pytorch/tnt.git@master
