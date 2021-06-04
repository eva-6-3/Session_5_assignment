# Observations from last Experiment
A lot of mistakes had to do with numbers with missing pixels (or written in such way), for eg ..    
![images of mistakes](https://github.com/askmuhsin/Session_5_assignment/blob/main/resources/exp_2_mistakes_2.png)

# Target:
* Analysis from last experiment, lead us to look into the data and how to improve the augmentations.
* in this experiment we are trying with RandomErasing of few pixels. (The reason explained in prev section of README)
  * `transforms.RandomErasing(p=0.5, scale=(0.02, 0.15), ratio=(0.3, 3.3), value=0)`
  * the probability of applying this transorm is 50% 
  * this transform when applied would cover an area of 2% to 15% of the image.
  * this transform would be of aspect ration ranging from a distribution of 0.3 to 3.3
* Sample of augmentation applied -- </br>
![without aug](https://github.com/askmuhsin/Session_5_assignment/blob/main/resources/no_aug.png) >> after aug >> 
![with aug](https://github.com/askmuhsin/Session_5_assignment/blob/main/resources/with_aug.png)

# Results:
* Parameters: 9,958
* Best Training Accuracy: 97.75% (EPOCH 15)
* Best Test Accuracy: 99.25 (EPOCH 14)

# Analysis:
* This model is able to rectify some of the mistakes done by previous models. 
* The augmentation seems to have helped.
* But with augmentation the Learning has become solwer, and inorder for it to fit will require more epochs.

# LOGS:
_Note -- batch_avg_training_acc is is the average of acc from all batches for an epoch_
![Training Log](https://github.com/askmuhsin/Session_5_assignment/blob/main/resources/exp_3_training_log.png)
