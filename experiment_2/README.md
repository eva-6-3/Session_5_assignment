# Target:
* Reduce some parameters in early blocks, and assign more towards later blocks.
	* Reduced channels in block 1, 2, 3 (Transition) as 6, 12, 7
	* Increased channels in block 4, 5, 6, 7 as 16, 16, 18, 18.

# Results:
* Parameters: 9,958
* Best Training Accuracy: 98.84% (EPOCH 15)
* Best Test Accuracy: 99.46% (EPOCH 14)

# Analysis:
* model has improved, and can see more stable test accuracy from epoch 14.
* it is still underfitting.

# LOGS:
_Note -- batch_avg_training_acc is is the average of acc from all batches for an epoch_
![Training Log](https://github.com/askmuhsin/Session_5_assignment/blob/main/resources/exp_2_training_log.png)
</br>Few epochs before and after max test acc</br>
![Highlight Log](https://github.com/askmuhsin/Session_5_assignment/blob/main/resources/exp_2_highlight_epochs.png)
</br>Model Architecture</br>
![Model Architecture](https://github.com/askmuhsin/Session_5_assignment/blob/main/resources/exp_2_model.png)

# ERRORS:
</br>Errors in Labeling from Model 2</br>
![part 1](https://github.com/askmuhsin/Session_5_assignment/blob/main/resources/exp_2_mistakes_1.png)
![part 2](https://github.com/askmuhsin/Session_5_assignment/blob/main/resources/exp_2_mistakes_2.png)
