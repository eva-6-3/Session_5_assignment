# Target:
* This run starts with the last best approach from class. but with the following changes -
  * Removing the LR Scheduler.
  * Reducing the Parameters to 10k. 
    * Reducing the size of initial Blocks.
		* 8 channel (B1) >> 16 channel (B2) >> 8 channel (TB1 / B3) 
    * No Changes made to the parameters in final blocks, as it is the understanding that there is more learning capacity required at final Blocks for this task.
		* 16 channel (B4) >> 16 channel (B5) >> 16 channel (B6) >>  16 channel (B7) >> 10 channel (out / B8)
* The intention of this step is to have the correct Setup and Parameters.

# Results:
* Parameters: 9,752
* Best Training Accuracy: 98.87% (EPOCH 15)
* Best Test Accuracy: 99.38% (EPOCH 13)       [99.41%   (EPOCH 16)]
 
# Analysis:
* The model showed a stable gap between train and test acc.
* But the model is underfitting, with potential to maybe learn with more epochs.
* The Validation accuracy does not have a huge variance in the last few epochs, but only once above 99.40%.  (variance of test acc in last 5 epochs - 0.0060)

# LOGS:
_Note -- epoch_avg_training_acc is is the average of acc from all batches for an epoch_
![Training Log](https://github.com/askmuhsin/Session_5_assignment/blob/main/resources/exp_1_training_log.png)
</br>Few epochs before and after max test acc</br>
![Highlight Log](https://github.com/askmuhsin/Session_5_assignment/blob/main/resources/exp_1_highlight_epochs.png)
</br>Model Architecture</br>
![Model Architecture](https://github.com/askmuhsin/Session_5_assignment/blob/main/resources/exp_1_model.png)
