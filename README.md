# Optimizing Crop Management with Reinforcement Learning and Imitation Learning

### 1. Dependencies
Follow https://rgautron.gitlabpages.inria.fr/gym-dssat-docs/Installation/index.html to install the required GYM-DSSAT.

### 2. Training

#### 2.1 Baselines
For RL-based policy training, the code can be found the folder of 'RL-based Training'. 

Run 
```bash 
Baseline.ipynb
```
to get the results of the baseline method for policy comparison. 

Run 
```bash 
Full_observation.ipynb
```
to train policies under full observation with custom weights using RL. Run 'Partial_onserbation.ipynb' to train policy under partial observtion with custom weights using RL.

#### 2.2 Partial Observation
For IL-based policy training, the code can be found the folder of 'IL-based Training'. 

Given a saved RL-trained policy (expert) under full observation, run
```bash 
Generate_data_set.ipynb
```
to obtain observation-action pairs for IL training. 

Once we obtain the dataset, run 
```bash 
IL-based_training.ipynb
```
to train policy under partial observbation using IL.


Given any trained policy, we can use the corresponding file from the folder of 'Policy Evalution' to evalute its performance. 
Use 
```bash 
IL-trained_partial.ipynb
```
to evalute IL-trained policies under partial observation. Use 'RL-trained_full.ipynb' to evalute RL-trained policies under full observation.

Use 
```bash 
RL-trained_partial.ipynb
```
to evalute RL-trained policies under partial observation.
