## This Repository
This repository contains the source code used for a research project in 
EPITA's Computer Science Master's program, to which the goal was to evaluate the
best performing neural network architecture, given a neuron constraint (i.e., 
resource budget).

The project heavily relies on [OpenAI's Baselines](https://github.com/openai/baselines) 
with only a few minor changes for the purpose of our experiment. 

## The Experiment
**Abstract**

We explore and evaluate the performance of different neural network architectures 
with a fixed neuron budget for deep reinforcement learning. We use a Double 
Dueling DQN algorithm with prioritized experience replay for the Atari game 
Space Breakers. We also use the default hyperparameters and frame stacking. 

**Experiment Overview**

We train our 3 agents for 10 million frames (or steps in the environment), 
which takes approximately 16 hours per agent on our testing computer. We 
conduct three experiments: first, a baseline consisting of a 4-layer MLP, 
second, a shallow network consisting of a 2-layer MLP, and third, 
a deep network consisting of a 8-layer MLP. We compare the different 
networks’ learning rate, measured by game play high score.

**The Results**

The agent with the deep 8-layer MLP performed the best with an average 
score of 250, but the outcome is relatively similar across all three 
experiments (baseline and shallow networks achieved average scores
of 242 and 247 respectively).

_To read more about the experiment, refer to 
[DDQN Research Report 2019-02-14.pdf](https://github.com/RedBanies3ofThem/baselines/blob/master/DDQNResearchReport2019-02-14.pdf))._

### Citing Our Research
To cite the original version of this repository in publications:

    @misc{Deep Reinforcement Learning,
      author = {Jonathan Sadighian, Nadia Sjöstedt, Rhea Moubarak},
      title = {Different Neural Network Depths for Deep Reinforcement Learning},
      year = {2019},
      publisher = {GitHub},
      journal = {GitHub repository},
      howpublished = {\url{https://github.com/RedBanies3ofThem/baselines}},
    }

