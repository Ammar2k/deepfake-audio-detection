# Deep Voice: Deepfake Voice Recognition

This repository contains a notebook for deepfake voice recognition using the Wav2Vec2 model from HuggingFace. The notebook is designed to process audio data, augment it to create a balanced dataset, and fine-tune the Wav2Vec2 and WeSpeaker model for voice recognition tasks.

## Table of Contents

1. [Data Preparation](#data-preparation)
2. [Data Augmentation](#data-augmentation)
3. [Audio Chunking](#audio-chunking)
4. [Data Preprocessing](#data-preprocessing)
5. [Model Fine-Tuning](#model-fine-tuning)

## Data Preparation

The notebook begins by connecting to HuggingFace to access pre-trained models. It then loads an example dataset from Kaggle, which is a deepfake voice recognition dataset. You should make your own bigger dataset for better performance.

## Data Augmentation

To address the class imbalance issue, the notebook augments the real voice data by adding random noise, time stretching, and pitch shifting. The augmented data is saved to the same directory as the original data.

## Audio Chunking

The audio files are then divided into 15-second chunks. This smaller segment size is suitable for training the model, as it allows for more efficient processing.

## Data Preprocessing

The audio data is preprocessed by resampling it to 16kHz and converting it to a mono channel. The preprocessed data is then saved to a new directory.

## Model Fine-Tuning

Finally, the notebook fine-tunes the Wav2Vec2 model using the preprocessed data. The model is fine-tuned to recognize voice characteristics and distinguish between real and fake voices.

Please refer to the notebook for detailed instructions on how to run the code and fine-tune the model for your specific use case.