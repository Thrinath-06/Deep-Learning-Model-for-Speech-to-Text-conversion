# Project Title
  Speech-to-Text Conversion 

# Contents

# Dataset Preparation:
- The dataset consists of audio files and their corresponding transcriptions.
- The dataset is downloaded and extracted from the specified URL.
- Audio files are collected and mapped to their transcriptions using a metadata file.
- A subset of the dataset is prepared based on the specified maximum transcription length.

# Data Exploration:
- Sample audio files are played, and their corresponding transcriptions are displayed for verification.

# Text Vectorization:
- A custom character-level vectorizer is implemented to convert transcriptions into numerical format.
- The vocabulary includes lowercase letters, spaces, and punctuation marks.
- The maximum length of transcriptions is specified, and longer texts are truncated.

# Model Architecture:
- The model architecture is based on the Transformer framework.
- The encoder processes audio features, transforming them into a suitable representation for the decoder.
- The decoder generates the transcription from the encoded audio features.
- The model is implemented using TensorFlow and Keras.

# Training:
- The model is trained using the prepared dataset.
- Loss function: CTC (Connectionist Temporal Classification) loss.
- Optimizer: Adam.
- Evaluation metrics:loss.
- The training loop runs for a specified number of epochs with progress tracking.

# Inference:
- Once trained, the model can be used to transcribe new audio files.
- The predicted transcriptions are displayed alongside the audio files for comparison.

# Evaluation:
- The performance of the model is evaluated using metrics such as  loss.
- Training progress and evaluation results are visualized by printing and comparing the output texts.

# Instructions:
- Download and extract the dataset using the provided script.
- Update the dataset path in the notebook.
- Ensure all dependencies are installed.
- Run the notebook to preprocess data, train the model, and generate transcriptions for new audio files.
- Modify the maximum transcription length and other parameters as needed.

# Dependencies:
- Python 3.x
- TensorFlow
- Keras
- NumPy
- IPython
- Glob
- IPython.display