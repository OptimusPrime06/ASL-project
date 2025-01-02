# American Sign Language Detection

## Project Description
This project is part of my AI course in college. It focuses on detecting American Sign Language (ASL) letters using machine learning techniques. The dataset consists of ASL photos representing the 26 letters of the alphabet, along with two additional classes: "nothing" and "space."
The primary goal of this project is to identify ASL letters as accurately as possible using two machine learning approaches:
1. **Convolutional Neural Networks (CNN)**
2. **Transfer Learning** with the **MobileNetV2** model. MobileNetV2 was chosen for its efficient resource usage and high performance.

## Table of contents
- [Project Description](#project-description)
- [Dataset](#dataset)
- [Files List](#files-list)
- [Technologies Used](#technologies-used)
- [System Requirements](#system-requirements)
- [Installation Instructions](#installation-instructions)
- [Usage Instructions](#usage-instructions)
- [Contributors](#contributors)
- [License](#license)

## Technologies Used
- **Programming Language**: Python
- **Frameworks and Libraries**: TensorFlow, Keras, and others listed in `requirements.txt`.

## System Requirements
- The project was developed and tested on a MacBook Air with an M3 chip. Performance may vary on other devices. 
- For Windows or Linux users, additional steps or libraries may be required to set up the environment, I will ensure to put as many steps as I can find.

## Installation Instructions
1. ### Clone the repository to your local machine:
   ```bash
   git clone <https://github.com/OptimusPrime06/ASL-project/>
   ```

2. ### Dataset 
   Download the dataset and put it in your project's directory
   <a href="https://www.kaggle.com/datasets/grassknoted/asl-alphabet" target="_blank">ASL Alphabet Dataset</a>
   ##### Notes:
   1. You will find a directory called asl_alphabet_train and asl_alphabet_test; you are allowed to delete the test dataset as it contain only 29 photos which is not enough at all to test our enormous dataset
   2. the dataset is divided into 29 directorie, 26 alphabetic letters, nothing, delete, and space. you can delete space it you want, I have deleted it as I felt it has no meanin but fine if you want to keep it you can do but you will make some changes in code.
   3. Each class of the 29 classeshas 3000 photos giving the total of 87,000 photos

3. ### Create the virtual environment
   ```bash
   cd <path to projects directory>
   python -m venv <your virtual environment name, commonly it is named venv>
   ```

4. ### Activate your virtual environment
   for macOS and Linux:
   ```bash
   source venv/bin/activate
   ```

   for Windows:
   ```bash
   venv\Scripts\activate
   ```

5. ### install required libraries from requirments.txt file
   ```bash
   pip install -r requirements.txt
   ```

 6. Install Jupyter Notebook extension for VScode
    here is a video that explains how to do it
    <a href="https://code.visualstudio.com/docs/datascience/jupyter-notebooks" target="_blank">Jupyter Notebook setup by VScode</a>

## Files List
1. [requirments.txt](requirments.txt)
2. [CNN.ipynb](CNN.ipynb)
3. [CNNClassificationReport.csv](CNNClassificationReport.csv)
4. [MobileNetV2.ipynb](MobileNetV2.ipynb)
5. [mobilenet_v2_weights_tf_dim_ordering_tf_kernels_1.0_224_no_top.h5](mobilenet_v2_weights_tf_dim_ordering_tf_kernels_1.0_224_no_top.h5)
6. [TransferLearningClassificationReport.csv](TransferLearningClassificationReport.csv)
7. [cnnASLModel.keras](cnnASLModel.keras)
8. [mobiletNetV2ASLModel.keras](mobiletNetV2ASLModel.keras)

## Usage Instructions
  1. Open the Python notebooks provided in the project directory.
  2. Read through the code to understand the workflow.
  3. Execute each cell sequentially to train and test the models.
  4. The results, including model performance and predictions, will appear in the notebook after training.

## Contributors
  1. Gulliver Raed aka OptimusPrime
  2. Special Thanks: <a href="https://github.com/Ziadahmed40" target="_blank">Ziad Ahmed</a> , for assistance in optimizing CNN model layers.

## License
This project is a term project and is not licensed for commercial use.


