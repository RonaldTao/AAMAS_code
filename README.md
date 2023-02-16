# 

Follow https://rgautron.gitlabpages.inria.fr/gym-dssat-docs/Installation/index.html to install the required GYM-DSSAT.

For RL-based policy training, the code can be found the folder of 'RL-based Training'. Run 'Baseline.ipynb' to get the results of the baseline method. Run 'Full_observation.ipynb' to train policies under full observation with custom weights using RL. Run 'Partial_onserbation.ipynb' to train policy under partial observtion with custom weights using RL.

For IL-based policy training, the code can be found the folder of 'IL-based Training'. Given a saved RL-trained policy (expert) under full observation, run 'Generate_data_set.ipynb' to obtain observation-action pairs for IL training. Once we obtain the dataset, run 'IL-based_training.ipynb' to train policy under partial observbation using IL.

Given any trained policy, we can use the corresponding file from the folder of 'Policy Evalution' to evalute its performance. 
