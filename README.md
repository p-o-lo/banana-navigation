# Banana Navigation
The repository contains an implementation of DQN (deep-Q-network) in order to train an agent for catching yellow bananas in a 2D space. 
A wide description of the Unity environments is on [Unity ML-Agents Toolkit](https://github.com/Unity-Technologies/ml-agents).


## Descritpion of the environment

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around agent's forward direction. 

The agent can choose 4 different actions:
- `0` - walk forward 
- `1` - walk backward
- `2` - turn left
- `3` - turn right

The aim is to collect as many yellow bananas as possible, avoiding the blue ones. A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. The agent will win the game if it gets an avarage reward of 13 for 100 episodes.


## Files provided

To make the project as readable as possible, only the **Navigation.ipynb** Python notebook is provided. In the netbook you will find a detailed description of the environment and the comments on the code 

The **report.pdf** describes the details of the implementation and more ideas about the DQN agent.

In order to run the code properlt a **python** folder is provided. In this folder there are all the files needed for the installation of the Unity environments. 


## Requirements and installation

To run the notebook firstly **Navigation.ipynb** we need to set up the environment as follow:

- Create (and activate) a new kernel with Python 3.6
    - **Linux** or **Mac**
   ```
   conda create --name drlnd python=3.6
   source activate drlnd
    ```  
    - **Windows**
   ```
    conda create --name drlnd python=3.6
    activate drlnd
   ```
- If you didn't before, you need a minimal install of OpenAI gym
```
pip install gym
pip install gym[classic_control]
pip install gym[box2d]
```
- Clone the repository, and navigate to the python/ folder. Then, install several dependencies.
```
git clone https://github.com/udacity/deep-reinforcement-learning.git
cd deep-reinforcement-learning/python
pip install .
```
- Create an IPython kernel for the dqn environment.
```
python -m ipykernel install --user --name drlnd --display-name "drlnd"
```
- Then you can finally open the **Navigation.ipynb**. Before running code in this notebook, change the kernel to match the drlnd environment by using the drop-down Kernel menu

![This is an image](https://user-images.githubusercontent.com/10624937/42386929-76f671f0-8106-11e8-9376-f17da2ae852e.png)
    
