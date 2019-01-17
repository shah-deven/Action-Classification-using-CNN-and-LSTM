# Action-Classification-using-CNN-and-LSTM

In this project, CNN - LSTM is trained to classify human actions. LSTMs are designed to handle sequential data.
For human action recognition, skeleton data is used that encodes the 3D locations of 25 body joints. The data is collected by Kinect v2. There are 10 different action classes. There are 4000 training sequences, 800 validation sequences, and 1000 test sequences. Each sequence has 15 frames, each frame is a 75-dimension vector (the xyz positions of 25 joints). <br> <br>

The following extra packages are required to run this:<br>
```
pip install h5py
pip install git+https://github.com/pytorch/tnt.git@master
```

**Network Architecture:** 2 layers of Convolution Neural Network along with 2 layers of Inception, upon it a single layer of LSTM with 50 hidden states.

**Optimizer:** Adadelta optimizer used because it reduces the learning rate dynamically with decaying rate 0.9

**Learning Rate:** 1e-1 Epochs used: 50


# Performance
Accuracy on Validation set achieved is 87%
Accuracy on Training set achieved is 100%
Loss on Validation set after 50th epoch is 0.5605
Loss on Training set after 50th epoch is 0.0034

# Kaggle Performance
Action Recognition using RNN - Rank 2 - `https://www.kaggle.com/c/cse512springhw5`
