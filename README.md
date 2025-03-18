# EEG Cognitive Load Analysis

## Overview
This project focuses on analyzing cognitive load using EEG data. It implements feature extraction, classification, and visualization using a CNN-LSTM model. The project also provides a GUI for easy interaction.

## Features
- Extract EEG features like band power, entropy, and coherence.
- Train a CNN-LSTM model for cognitive load classification.
- Predict cognitive load based on EEG recordings.
- Compare cognitive load between different groups.
- Visualize results using bar charts and confusion matrices.

## Installation
### Prerequisites
Ensure you have Python installed (>= 3.7). Install the required dependencies using the following command:

```sh
pip install -r requirements.txt
```

## Usage
1. Run the GUI application:
   ```sh
   python main.py
   ```
2. Use the interface to predict cognitive load from EEG data or compare different groups.

## Data Format
- EEG data should be in CSV format with rows representing time-series samples and columns representing EEG channels.
- Store datasets in separate folders for different groups.

## Model Training
- If a trained model (`eeg_cnn_lstm_model.h5`) is not found, the script will train a new model.
- Training data should be placed in the `Active state` directory.

## File Structure
```
|-- main.py             # Main script with GUI & model
|-- eeg_cnn_lstm_model.h5  # Trained model (generated after training)
|-- requirements.txt    # Dependencies
|-- data/               # Folder to store EEG datasets
```

## Dependencies
Refer to `requirements.txt` for all required packages.

## License
This project is open-source and free to use.

