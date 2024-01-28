# DeepFake Audio Detection

This repository will walk you through how to fine-tune a deepfake audio detection classification module.

First step is to setup your dataset in the following way:
Dataset
    test
        fake
        real
    train
        fake
        real

After the dataset has been loaded in, import a pre-trained model from HuggingFace, set up PyTorch DataLoaders, and run the model through a training loop.

The results are then evaluated and the hyper-parameters are optimized.