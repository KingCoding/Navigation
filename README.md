# NAVIGATION
![Continuous Control snapshot](https://github.com/KingCoding/Continuous-Control-Optimized-Sampling/blob/main/pictures/Continuous%20Control%20Snapshot.png)
## DESCRIPTION
Uses DQN a reinforcement learning algorithm to solve a navigation environment where an agent's goal is to collect the maximum number of bananas
The goal pf this project is to train an agent to navigate (and collect bananas!) in a large, square world.
A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. Thus, the goal of your agent is to collect as many yellow bananas as possible while avoiding blue bananas.

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around the agent's forward direction. Given this information, the agent has to learn how to best select actions. Four discrete actions are available, corresponding to:

0 - move forward.
1 - move backward.
2 - turn left.
3 - turn right.
The task is episodic, and in order to solve the environment, your agent must get an average score of +13 over 100 consecutive episodes.

## REQUIREMENT AND SETUP
To set up your python environment to run the code in this repository, follow the instructions below.\
1- Create (and activate) a new environment with Python 3.6.
- **Linux** or **Mac:**
  ```
  conda create --name drlnd python=3.6
  source activate drlnd
  ```
- ***Windows:***
  ```
  conda create --name drlnd python=3.6 
  activate drlnd
  ```

2- Install OpenAi gym from [this repository](https://github.com/openai/gym)
- install the classic control environment group through [this link](https://github.com/openai/gym#classic-control)
- install the box2d environment group through [this link](https://github.com/openai/gym#box2d)

3- If you haven't yet done it, clone this repository, then navigate to the main Navigation/ folder.\
   There is no need to run the command pip install . in order to make initial python installation, because the main project file does it first
  ```
  git clone https://github.com/KingCoding/Navigation.git
  cd Navigation
  ```
4- Download the Unity environment for this project that mathes your operating system:
- Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
- Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
- Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
- Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)

(For Windows users) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

(For AWS) If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Linux_NoVis.zip) to obtain the "headless" version of the environment. You will not be able to watch the agent without enabling a virtual screen, but you will be able to train the agent. (To watch the agent, you should follow the instructions to [enable a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md), and then download the environment for the Linux operating system above.)


5- In the Navigation/ repository folder, unzip (or decompress) the downloaded Unity environment file.

6- Open the Navigation.ipynb file and replace the unity environment file name with the name of the unity environment corresponding to your plateform that you have donwloaded
```
change this line:
env = UnityEnvironment(file_name="/data/Banana_Linux_NoVis/Banana.x86_64")
with this:
env = UnityEnvironment(file_name="YOUR_SYSTEM_UNITY_ENVIRONMENT_FILE_NAME")
```

## EXECUTION
Run all the intructions in the Continuous_Control_Optimized_Sampling.ipynb file to train the Navigation agent.

## TRAINING RESULT GRAPH
![Training result graph](https://github.com/KingCoding/Continuous-Control-Optimized-Sampling/blob/main/pictures/Continuous%20Control%20Chart.png)
