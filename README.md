# Unity ML-Agents Navigation

## Project Details
For this project, you will train an agent to navigate (and collect bananas!) in a large, square world.

![banana](https://user-images.githubusercontent.com/4464676/74794975-fa73f000-5307-11ea-9bd1-ecfc84740e60.gif)

A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. Thus, the goal of your agent is to collect as many yellow bananas as possible while avoiding blue bananas.

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around the agent's forward direction. Given this information, the agent has to learn how to best select actions. Four discrete actions are available, corresponding to:

- `0` - move forward.
- `1` - move backward.
- `2` - turn left.
- `3` - turn right.  
The task is episodic, and in order to solve the environment, your agent must get an average score of +13 over 100 consecutive episodes.


## Getting Started  

* This repository is only for Windows 10 (64-bit).  *

### Step 1
Follow this [instructions](https://github.com/udacity/deep-reinforcement-learning#dependencies) to set up your Python environments.


### Step 2

For this project, you will not need to install Unity - this is because we have already built the environment for you, and you can download it from the [link here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip).


Then, place the file in the p1_navigation/ folder in the DRLND GitHub repository, and unzip (or decompress) the file.

(For Windows users) Check out this link if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

(For AWS) If you'd like to train the agent on AWS (and have not enabled a virtual screen), then please use this link to obtain the "headless" version of the environment. You will not be able to watch the agent without enabling a virtual screen, but you will be able to train the agent. (To watch the agent, you should follow the instructions to enable a virtual screen, and then download the environment for the Linux operating system above.)

Step 3: Explore the Environment
After you have followed the instructions above, open Navigation.ipynb (located in the p1_navigation/ folder in the DRLND GitHub repository) and follow the instructions to learn how to use the Python API to control the agent.

Watch the (silent) video below to see what kind of output to expect from the notebook, if everything is working properly!


In the last code cell of the notebook, you'll learn how to design and observe an agent that always selects random actions at each timestep. Your goal in this project is to create an agent that performs much better!
