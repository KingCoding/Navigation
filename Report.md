## INTRODUCTION
Took most time to understand the DQN algorithm. But afterward, the application was straightforward.

## LEARNING ALGORITHM
Deep Q-Network (DQN) algorithm

### Networks configuration
- Number of local network = 1
- Number of target network = 1 
- Size of local network = (37, 64, 64, 4)
- Size of target network = (37, 64, 64, 4)
- rate for soft update of target TAU = 1e-3

### Hyperparameters
- Replay buffer size = 1e5
- Minibatch size = 64
- Discount factor = 0.99
- Soft update of target parameters coefficient(TAU) = 1e-3
- Local network learning rate = 5e-4
- Target network learning rate = 5e-4
- How often to update the network (time steps) = 4
==

The max reward achieved during training was 13.02 at episode 548.

![Training Result Graph](https://github.com/KingCoding/Navigation/blob/main/pictures/Navigation_Result_Graph.png)
...

## IDEAS FOR FUTURE WORK
- Try different hypeparameters like network sizes, batch size,...

- Try a different algorithm other than the DQN algorithm
