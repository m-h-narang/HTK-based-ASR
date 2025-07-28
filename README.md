# HTK-based ASR Demonstrator — Dutch Postcode Recognition

This project implements a speaker-dependent Automatic Speech Recognition (ASR) system using the HTK toolkit to recognize Dutch postcodes. The recognizer is trained on self-recorded speech data and demonstrates recognition of postcodes in the format four digits followed by two capital letters (e.g., 8911 CE).
The work was conducted as part of the Voice Technology MSc. 2024–2025 Speech Recognition 1 course at the University of Groningen.

---

## Original Toolkit

The full HTK toolkit can be obtained from:

http://htk.eng.cam.ac.uk/

---

## Project Description

This project focuses on building a speaker-dependent HTK-based ASR system and includes the following tasks:

- Recording custom training data for each group member using the provided microphone setup
- Training Hidden Markov Models (HMMs) to recognize Dutch postcodes spoken digit by digit and letter by letter
- Configuring pronunciation dictionaries, language models, and HMMs for postcode recognition
- Performing live demonstrations where each group member speaks randomly generated postcodes, and the recognizer outputs predicted sequences
- Evaluating performance using Word Error Rate (WER)

---

## What This Repository Contains

This folder only includes modified or newly created files relevant to the project.
To access the full HTK toolkit and example scripts, download HTK from the official website linked above.

Key elements in this project include:

- Recorded training and validation datasets for Dutch postcodes
- HMM definitions and trained model files
- Word network, dictionary, and grammar files for postcode recognition
- Scripts to run training, recognition, and evaluation
- A configuration file (group_config.yml) for grading and demonstration

---

## How to Run

1. Install HTK

Follow the installation instructions from the HTK website to build and install the toolkit.

2. Prepare Data

Record training data for the target speaker following the postcode format, ensuring audio is mono, 48kHz, 16-bit WAV.

3. Extract Features

Use HTK tools such as HCopy to extract MFCC features from the recorded data.

4. Train HMM Models

Run the provided training scripts to initialize and iteratively re-estimate HMMs for digits and letters.

5. Perform Recognition

Use HVite with the trained models, dictionary, and word network to recognize spoken postcodes.

6. Evaluate WER

Compare recognized sequences with reference labels to compute the Word Error Rate (WER) using HTK or the provided Python script.

---

## Language

The project was developed for Dutch postcode recognition using English letter names and digit pronunciations spelled out in words.



