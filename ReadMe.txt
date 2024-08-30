
Project Overview: 234101036_DigitRecognition

This project, 234101036_DigitRecognition, was created using Visual C++ with the help of the Application Wizard. Below is a summary of the key files and their purposes within the project.

Project Files

- 234101036_DigitRecognition.vcxproj 
  This file is the primary project file for the VC++ application. It contains essential information about the version of Visual C++ used, as well as the platforms, configurations, and project settings selected during the creation process.

- 234101036_DigitRecognition.vcxproj.filters 
  This file manages the association between the project files and their respective filters. It helps organize files with similar extensions under specific categories (e.g., ".cpp" files under the "Source Files" filter) in the IDE.

- 234101036_DigitRecognition.cpp 
  This is the main source file containing the primary application logic.

Additional Standard Files

- StdAfx.h, StdAfx.cpp  
  These files are used to generate a precompiled header (PCH) file named `234101036_DigitRecognition.pch` and a precompiled types file named `StdAfx.obj`.

Notes

The Application Wizard includes "TODO:" comments throughout the source code to indicate sections that may require customization or further implementation.

Modular Functions

The code is structured into several modular functions that are utilized within the main function. Below are the primary functions:

- readuniverse()  
  Reads the universe data from the `universe.txt` file.

- LBG() 
  Implements the Linde-Buzo-Gray (LBG) algorithm to generate a codebook of size 32 using the universe data read by the `readuniverse()` function.

- training_model()  
  Trains Hidden Markov Models (HMMs) using the training dataset (i.e., the first 25 utterances of each digit) and generates the final models for each digit.

- testing_model()  
  Tests the trained models using the test dataset (i.e., utterances 20 to 30 of each digit) and displays the accuracy along with the probability of correct digit recognition.

- liveTesting()  
  Records spoken digits in real-time and recognizes the digit based on the trained models.

- readCodebook()  
  Loads the final codebook into the `codebook` array to generate observation sequences for the input files.

- create_observation_sequence()  
  Creates observation sequences and stores them in the `ob[]` array.

Project Structure

- dataset/  
  Contains the dataset used for training and testing.

- lamda_new/  
  Stores the trained HMM models.

- obs_seq/  
  Stores the generated observation sequences.

--- 

This readme provides a clear and original summary of the project's structure and components.