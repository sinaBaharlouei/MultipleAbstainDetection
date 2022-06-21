# Improving adversarial robustness via  joint classification and multiple explicit detection classes
We improved the trade-off between natural accuracy and robust  verifiable accuracy by introducing multiple abstain classes to the training and verification procedures
of neural networks. 

## Run 


To train the network with multiple abstain classes for the CIFAR-10 dataset with epsilon=12/255, run the following:

```python train.py "training_params:method=robust_natural" "training_params:method_params:bound_type=interval" --config config/cifar_dm-shallow_12_255.json```


In the config file you can assign parameters such as M (the number of abstain classes), gamma (the hyper-parameter for the regularization), is_regularized (whether you wan to regularize model to have balance between classes), and alpha (the step-size for the Bergman divergence).


