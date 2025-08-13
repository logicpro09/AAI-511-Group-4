# AAI-511-Group-4
# Composer Classification Using Symbolic Music Data

**Group Members:** Ahmed Salem, Ramesh Dhanasekaran, Victor Salcedo  

## Overview
This project classifies classical music composers from MIDI data.  
Three models were developed:  
1. Convolutional Neural Network (CNN)  
2. Long Short-Term Memory Network (LSTM)  
3. Hybrid CNN–LSTM  

The hybrid model achieved the best results.

## Dataset
- MIDI files from four composers: **Bach, Beethoven, Chopin, Mozart**  
- Extracted pitch-class histograms for CNN  
- Extracted note and chord sequences for LSTM and Hybrid models  
- Applied data augmentation with pitch transposition and tempo scaling  

## Methodology
- Preprocess features with normalization and label encoding  
- Split into 80% training and 20% testing  
- Apply class weighting to handle imbalance  
- Train CNN, LSTM, and Hybrid models  
- Evaluate with accuracy, precision, recall, and F1-score  

## Results

| Model               | Accuracy | Precision | Recall | F1-Score |
|---------------------|----------|-----------|--------|----------|
| CNN                 | 0.68     | —         | —      | —        |
| LSTM                | 0.66     | 0.66      | 0.66   | 0.66     |
| Hybrid CNN–LSTM     | 0.97     | 0.97      | 0.97   | 0.97     |

The hybrid model outperformed others on all metrics.

## Requirements
- Python 3.9 or newer  
- TensorFlow  
- scikit-learn  
- pandas  
- numpy  
- matplotlib  
- seaborn  
- music21  

## How to Run
1. Clone this repository  
2. Install dependencies:
    
    ```bash
    pip install -r requirements.txt
    ```
3. Run the notebook in Google Colab or Jupyter  
4. Follow the preprocessing and training sections in the notebook  
5. Evaluate models with provided scripts  

## Future Improvements
- Add more composers  
- Include rhythmic and harmonic features  
- Experiment with Transformer-based models  
- Use cross-validation and ensembling  
- Develop real-time composer classification tools  
