# TinyML for Emotion Detection in Voice Signals  

This repository contains the code, datasets, and documentation for the research project titled **"TinyML for Emotion Detection in Voice Signals: Evaluating and Proposing Algorithms for IoT Wearable Devices"**. The project explores the use of Tiny Machine Learning (TinyML) to implement voice emotion recognition models optimized for resource-constrained IoT devices such as wearables.  

---

## Overview  
Voice emotion recognition is critical for applications like healthcare, human-computer interaction, and IoT technologies. This project evaluates machine learning models (BiLSTM, CNN, LSTM, GRU) on composite datasets and deploys the best-performing models using TensorFlow Lite on Raspberry Pi for real-time, power-efficient processing.  

---

## Features  
- **Advanced ML Models:** Includes implementations of BiLSTM, CNN, LSTM, and GRU for speech emotion recognition.  
- **Optimized Deployment:** TensorFlow Lite models for deployment on resource-constrained hardware.  
- **Composite Datasets:** Uses diverse datasets (RAVDESS, CREMA-D, TESS, SAVEE) for training and evaluation.  
- **Real-Time Applications:** Demonstrates real-time emotion detection on Raspberry Pi 4B.  

---

## Datasets  
The research used publicly available datasets for emotion recognition:  
1. **[RAVDESS](https://zenodo.org/record/1188976)**  
2. **[CREMA-D](https://github.com/CheyneyComputerScience/CREMA-D)**  
3. **[TESS](https://tspace.library.utoronto.ca/handle/1807/24487)**  
4. **[SAVEE](http://kahlan.eps.surrey.ac.uk/savee/)**  

For preprocessing, we extracted features like Mel-Frequency Cepstral Coefficients (MFCC), Zero Crossing Rate, and Root Mean Square Energy (RMSE).  

---

## Getting Started  

### Prerequisites  
- Python 3.8+  
- TensorFlow 2.10+  
- TensorFlow Lite  
- Raspberry Pi (for hardware deployment)  

### Installation  
1. Clone the repository:  
   ```bash
   git clone https://github.com/your-username/emotion-detection-tinyml.git
   cd emotion-detection-tinyml
2. Install dependencies:
   pip install -r requirements.txt
3. Running the Models
Train Models:
Use the provided train_model.py script to train the models:
python train_model.py --model BiLSTM --epochs 50
4. Evaluate Models:
Run evaluate_model.py to calculate accuracy, precision, and recall:
  python evaluate_model.py --model BiLSTM
5. Deploy on Raspberry Pi:
Follow the instructions in the hardware/ directory to convert the model to TensorFlow Lite and deploy it on Raspberry Pi.


## Results
The best-performing models achieved the following accuracy:

**Model	Accuracy**
- **BiLSTM	88%**
- **CNN	85%**
- **LSTM	86%**
- **GRU	82%**

## Hardware Implementation
The TensorFlow Lite models were tested on a Raspberry Pi 4B with the following specifications:

- **Quad-core Cortex-A72 CPU**
- **8GB LPDDR4 RAM**
- **External microphone and sound card**
Refer to the hardware/ folder for step-by-step deployment instructions and performance benchmarks.

## Future Work
- **Integrate multi-modal data (audio, visual cues) for enhanced emotion detection**
- **Optimize models further for ultra-low-power devices**
- **Explore applications in mental health monitoring and social interaction analysis**

## Contact
For any queries or collaboration opportunities, feel free to reach out:
Email: tshewangchoden71@gmail.com

