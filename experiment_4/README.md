# Target:
* Increase LR to .02
* Remove Dropout
* Background
  * Last model was trained on a dataset with more augmentation, and therefore was taking more epochs to converge.
  * Now Trying with a higher learning rate, in order to get desired accuracy within 15 epochs.

# Results:
* Parameters: 9,958
* Best Training Accuracy: 98.53% (EPOCH 15)
* Best Test Accuracy: 99.42% (EPOCH 10)

# Analysis:
* By removing Dropout and increasing learning rate to 0.20 the test accuracy has reached 99.42% stably.

# LOGS:
_Note -- batch_avg_training_acc is is the average of acc from all batches for an epoch_ 
![Training Log](https://github.com/askmuhsin/Session_5_assignment/blob/main/resources/exp_4_training_logs.png)
</br>Few epochs before and after max test acc</br>
![Highlight Log](https://github.com/askmuhsin/Session_5_assignment/blob/main/resources/exp_4_highlight_epochs.png)

# ERRORS:
</br>Errors in Labeling from Model 2</br>
![part 1](https://github.com/askmuhsin/Session_5_assignment/blob/main/resources/exp_4_mistakes_1.png)
![part 2](https://github.com/askmuhsin/Session_5_assignment/blob/main/resources/exp_4_mistakes_2.png)

