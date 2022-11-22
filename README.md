# resnet_modified
Modifying ResNet18 from the following repository to give higher accuracy for &lt;5M parameters

https://github.com/kuangliu/pytorch-cifar

Our experiments for 40 epochs in the main file include:

- Reducing number of residual blocks
- Reducing number of residual layers and residual blocks
- Reducing number of residual layers, blocks and increasing number of channels
- Reducing number of residual layers, blocks, increasing number of channels and modifying average pool kernel size 
- Same configuration as configuration 3 but changing number of channels in the initial residual layer
- Same configuration as configuration 4 but changing number of channels in the initial residual layer

We also experimented with bottleneck, with more epochs, using SGD as optimizer instead of Adam and auto-augment policy for image transformation which can be found in our experiments folder. 

Instructions for running: 

1. You can run the main mini_project.ipynb file for all the 6 configurations discussed above trained for 40 epochs. 
2. You can use the models from the models folder to save time running the visualization and evaluation section. 
3. You can checkout our experiments folder for other configuration change experiments not included in the main notebook. 
4. You can refer the output folder for all the main configuration training runs snapshot. 
5. configuration2_100epochs.ipynb has the followup run for configuration 2 (our best model) with 100 epochs. 
