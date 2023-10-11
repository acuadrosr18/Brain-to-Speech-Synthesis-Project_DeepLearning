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
As students, we will study the BRAIN2SPEECH domain and then develop and train new types of neural network architectures.
The data implemented in the project is the **Dataset of Speech Production in intracranial Electroencephalography** (SingleWordProductionDutch), available [here](https://osf.io/nrgx6/)

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
- Data preparation for training, validation and test.

In the **Brain-to-Speech-Synthesis-Project_DeepLearning** Github Repository we can find the README.md file with the summary of the project, and the .IPYNB file which contains the resolution of the Milestone #1 of the project.

