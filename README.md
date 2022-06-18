# CS275-Simulating-Reinforcement-Learning-for-Locomotion-Control-of-Bipedal-Robots

In this project, we have used the A3C and DDPG algorithms to traim the controller of a Bipedal robot. Our physics-based character's locomotion skills will not just target flat terrain, but also more difficult terrain. Our goal in this research is to learn controllers that allow simulated characters to move through complex terrains with gaps, slopes, steps, and barriers while maintaining highly dynamic gaits. A reinforcement learning approach and an evolution strategy will be used to teach such terrain-adaptive locomotion skills.

## Group Members
* Pranjal Jain
* Sahil Bansal
* Siddarth Krishnamoorthy
* Gautam Dudeja

## Dependencies
* gym
* torch
* box2d-py
* evostra
* glfw
* h5py
* numpy
* Pillow
* PyOpenGL
* scipy
* six

## Run the code

To run the A3C code, go into the /a3c directory and test our pre-trained BipedalWalker-v2 controller using the command
* make demo-simple

To test our pre-trained BipedalWalkerHardcore-v2 controller, run the command
* make demo-hardcore

If you want to train your own model, here is an example
* python3 ./src/main.py --mode=train --env="BipedalWalker-v2" --n_workers=4 --n_frames=1 --n_steps=20 --model_load_dir="./models/CS275-BipedalWalker-v2" --model_save_dir="./models/new-BipedalWalker-v2"


To run the DDPG algorithm, the code is present in the /bipedal-walker/ddpg-torch directory. Then the following comman an be called
* python3 train.py 

The flag pretrained can be set to true to in order to use our pretrained model. Else, the model trains from scratch. 
