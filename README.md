# DeepFake Audio Detection

This repository will walk you through how to fine-tune a deepfake audio detection classification module.

The first step is to load the dataset, pre-process it, and load it into PyTorch Dataloaders.

After the dataset has been loaded in, import a pre-trained model from HuggingFace, define hyper-parameters, and run the model through a training loop.

The results are then evaluated and the hyper-parameters are optimized.