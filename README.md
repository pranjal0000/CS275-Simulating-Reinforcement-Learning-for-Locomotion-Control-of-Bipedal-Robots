# CS275-Simulating-Reinforcement-Learning-for-Locomotion-Control-of-Bipedal-Robots

In this project, we have used the A3C and DDPG algorithms to traim the controller of a Bipedal robot. Our physics-based character's locomotion skills will not just target flat terrain, but also more difficult terrain. Our goal in this research is to learn controllers that allow simulated characters to move through complex terrains with gaps, slopes, steps, and barriers while maintaining highly dynamic gaits. A reinforcement learning approach and an evolution strategy will be used to teach such terrain-adaptive locomotion skills.

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
$ make demo-simple
