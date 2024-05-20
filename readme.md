# Neural Machine Translation - A Comparative Performance Analysis of RNN, LSTM, and GRU

## Overview

This repository contains the code and data for the CS455 Semester Project titled "Neural Machine 
Translation - A Comparative Performance Analysis of RNN, LSTM, and GRU". The project provides a 
comprehensive performance analysis of three prominent neural network architectures: Recurrent 
Neural Networks (RNNs), Long Short-Term Memory (LSTM) networks, and Gated Recurrent Units (GRUs) 
in the domain of machine translation. The study focuses on the translation of French to English 
using a parallel corpus.

## Authors

- Muhammad Farae, Faculty of Computer Science & Engineering, Ghulam Ishaq Khan Institute of 
Engineering Sciences and Technology, Topi, Pakistan. Email: u2020292@giki.edu.pk
- Uzair Rahman, Faculty of Computer Science & Engineering, Ghulam Ishaq Khan Institute of 
Engineering Sciences and Technology, Topi, Pakistan. Email: u2020509@giki.edu.pk

## Abstract

This study evaluates the performance of RNN, LSTM, and GRU architectures in neural machine 
translation tasks. Performance metrics include translation accuracy, training time, and the 
ability to handle long sequence dependencies. The results aim to guide future research and 
practical implementations in neural machine translation, particularly for applications requiring 
efficient and accurate cross-lingual communication.

## Methodology

1. **Data Preparation**: 
    - A parallel corpus of French to English translations was sourced from a publicly available 
dataset.
    - Preprocessing steps included tokenization, vocabulary building, padding, and 
vectorization.

2. **Models Implemented**:
    - **Recurrent Neural Networks (RNNs)**: Basic neural networks capable of processing 
sequences but struggling with long-term dependencies.
    - **Long Short-Term Memory (LSTM) networks**: Advanced RNN variant that handles long-range 
dependencies using gating mechanisms.
    - **Gated Recurrent Units (GRUs)**: Similar to LSTMs but with a simpler structure, leading 
to faster training times.

3. **Evaluation Metrics**:
    - BLEU and ROUGE scores for translation accuracy.
    - Training time and computational efficiency.
    - Ability to handle long sentence structures and contextual dependencies.

## Results

- **LSTM** achieved the highest BLEU score and performed best across all ROUGE metrics, 
indicating superior translation quality and handling of complex linguistic structures.
- **GRU** showed reasonable performance but lagged behind LSTM in handling complex translations.
- **RNN** had the lowest performance, struggling significantly with the complexities of language 
translation.

## Conclusion

The study highlights the importance of selecting the appropriate neural network architecture for 
machine translation tasks. LSTM networks demonstrated the best performance, followed by GRUs, 
with RNNs being the least effective. Future research could explore incorporating attention 
mechanisms, hybrid models, and larger datasets with varied language pairs.

## Usage

1. **Clone the repository**:
    ```sh
    git clone https://github.com/yourusername/nmt-comparative-analysis.git
    cd nmt-comparative-analysis
    ```

2. **Install dependencies**:
    ```sh
    pip install -r requirements.txt
    ```

3. **Download the dataset**:
    - The dataset can be obtained from [this link](https://go.aws/38ECHUB).
    - Place the dataset in the `data` directory.

4. **Preprocess the data**:
    ```sh
    python preprocess.py
    ```

