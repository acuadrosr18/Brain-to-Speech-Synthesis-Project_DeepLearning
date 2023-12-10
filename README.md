# Brain-to-Speech Synthesis Project

## Team Name: 
  The AI Alchemists
## Team Members:
  1. Cuadros Rivas, Alejandra Paola - KK5459
  2. Konyakin, Dmitriy - JHGBFA
  3. Xu, Yang - LYQU2F

## Project Description
The purpose of a brain-computer interface (BCI) is to provide a natural or near-natural channel of communication for people who cannot speak due to physical or neurological impairment.
Speech is the primary and most essential means of human communication. However, many people have lost this ability through illness or ill health. The real-time synthesis of speech directly from measured neural activity (BRAIN2SPEECH) would enable natural speech and significantly improve quality of life, especially for severely communication-impaired individuals.
The data implemented in the project is the **Dataset of Speech Production in intracranial Electroencephalography** (SingleWordProductionDutch), available [here](https://osf.io/nrgx6/)

As students, we will study the BRAIN2SPEECH domain and then develop and train new types of neural network architectures.

About the **experimental design** for the dataset, in the study, participants were asked to read aloud words that were shown in their laptop screen, one random word from the stimulus library was presented on the screen for two seconds  while they read it aloud once. This procedure was repeated for a total od 100 words, resulting of 300 seconds for each participant (Verwoert, Ottenhoff, Goulis, et al., 2022).

For the **data acquisition**, articipants were implanted with platinum-iridium sEEG electrode shafts (Microdeep intracerebral electrodes; Dixi Medical, Beçanson, France) with a diameter of 0.8 mm, a contact length of 2 mm and a inter-contact distance of 1.5 mm. Each electrode shaft contained between 5 and 18 electrode contacts. Neural data was recorded using two or more Micromed SD LTM amplifier(s) (Micromed S.p.A., Treviso, Italy) with 64 channels each. Electrode contacts were referenced to a common white matter contact. Data were recorded at either 1024 Hz or 2048 Hz and subsequently downsampled to 1024 Hz. They used the onboard microphone of the recording notebook (HP Probook) to record audio at 48 kHz. Audio data was subsequently pitch-shifted to ensure our participants’ anonymity using LibRosa63. They used LabStreamingLayer64 to synchronize the neural, audio and stimulus data (Verwoert, Ottenhoff, Goulis, et al., 2022)

The related dataset contains a recontruction of the log-mel spectrogram from the high-frequency features using linear regression models. In these models, the high-frequency feature vector is multiplied with a weight matrix to reconstruct the log-mel spectrogram. The weights are determined using a least-squares approach.

As part of the project we will replace the linear regression model with deep neural networks considering one single speaker.

> Related materials:
> - [Single Word Production - Github](https://github.com/neuralinterfacinglab/SingleWordProductionDutch)
> - M. Verwoert, M. C. Ottenhoff, S. Goulis, A. J. Colon, L. Wagner, S. Tousseyn, J. P. van Dijk, P. L. Kubben, and C. Herff, “Dataset of Speech Production in intracranial Electroencephalography,” Scientific Data 2022 9:1, vol. 9, no. 1, pp. 1–9, jul 2022. [Online](https://www.nature.com/articles/s41597-022-01542-9)

# Milestone 1: Data acquisition, Data preparation - 2023.10.11

- Data source
- Data exploration and visualization 
- Data preparation for training

In the **Brain-to-Speech-Synthesis-Project_DeepLearning** Github Repository we can find the README.md file with the summary of the project, and the .IPYNB file which contains the resolution of the Milestone #1 of the project.

# Milestone 2: Baseline evaluation, Baseline model 2023.11.08
- Efficient loading of data
- Deep learning model: SpectrogramReconstructionNet
- Evaluation: For Linear Regression and for Deep Learning Model.

## How to Run the Pipeline
Detailed instructions on how to run the pipeline are as follows:

1. Installation:
Ensure you have Python installed and then set up the environment using the `requirements.txt` file as shown above.
 
2. Data Loading:
This notebook contains all necessary code to load the data.
 
3. Model Training:
This notebook contains all necessary code and displays the results inline.

4. Evaluation:
It will output evaluation metrics and optionally, visualizations comparing true values against predictions.

5. Application:
At the end, the best model will me applied to reconstruct a Spectrogram.

As we can see in the images, the reconstruction of the Spectrogram was succesful, the model performance was effective.

![image](https://github.com/acuadrosr18/Brain-to-Speech-Synthesis-Project_DeepLearning/assets/15305050/6809c140-dcd5-46e3-8c42-858ae35383e8)
![image](https://github.com/acuadrosr18/Brain-to-Speech-Synthesis-Project_DeepLearning/assets/15305050/ddb67ac7-05d4-4e8a-96a1-23daf1b3947f)

### Running the Training
This notebook includes:
- Data preprocessing.
- Model definition and setup.
- The training loop with output metrics.

### Running the Evaluation
For evaluation this code will:
- Load the best performing model.
- Run the model against the test data.
- Output the evaluation metrics.
- Include visualizations of results.

# Documentation:
This project's documentation provides an overview of an approach to audio signal processing, specifically the reconstruction of spectrograms from neural data.

It outlines our methods, from preprocessing to model evaluation, and discusses the practical applications of our findings. 

Guide to the project setup, execution, and results, ensuring clarity and ease of use for future development and collaboration.

[Brain-to-Speech-Synthesis Project Documentation](Brain-to-Speech-Synthesis-Project_DeepLearning.pdf)

