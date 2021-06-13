# Target:
* Add Dropout of 0.05
* Start with LR at 0.02, and ReduceLROnPlateau with a reduction factor of 0.5 when no imporvement in `test_loss` for 2 Epochs. Since the factor is a bit high setting min_lr to 0.001
 
# Results:
* Parameters: 9,958
* Best Training Accuracy: 98.35% (EPOCH 14)
* Best Test Accuracy: 99.46% (EPOCH 13) 99.48 (EPOCH 19)
 
# Analysis:
* by adding step lr and Dropout of 0.05, the training is even more stable.
* consistent test accuracy around 99.4 observed from epoch 13.
* The LR was reduced at EPOCH 12.
* Since the model is underfitting till EPOCH 20, training for more epochs OR removing regularizations would be helpful.
