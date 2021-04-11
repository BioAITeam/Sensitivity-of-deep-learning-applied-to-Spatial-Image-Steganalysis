# Sensitivity of Deep Learning Applied to Spatial Image Steganalysis
In recent years, the traditional approach to spatial image steganalysis has shifted to Deep Learning (DL) techniques, which have improved the detection accuracy while combining feature extraction and classification in a single model, usually, a Convolutional Neural Network (CNN). The main contribution from researchers in this area are new architectures that further improve the detection accuracy. Nevertheless, the preprocessing and partition of the database influence the overall performance of the CNN. This paper presents the results achieved by novel steganalysis networks (Xu-Net, Ye-Net, Yedroudj-Net, SR-Net, Zhu-Net, and GBRAS-Net) using different combinations of image and filter normalization ranges, various database splits, a diverse composition of the training mini-batches, different activation functions for the preprocessing stage, as well as an analysis on the activation maps and how to report accuracy. These results demonstrate how sensible steganalysis systems are to changes in any stage of the process and how important it is for researchers in this field to register and report their work thoroughly. We also propose a set of recommendations for the design of experiments in steganalysis with DL.
## Folders
- **Activation maps** This folder contains a notebook for getting Ye-Net activation maps.
- **CNN input** This folder contains the notebook Ye-Net  with three different approaches; Usual(providing all the cover images, then all the stego images), Random(random positions of cover and stego images), and order (alter-nates cover and stego images).
- **Database partition** This folder contains the notebooks Xu-Net, Ye-Net, Yedroudj-Net, SR-Net, Zhu-Net, and GBRAS-Net with different data partitions.
- **Image normalization** This folder contains the notebooks Xu-Net, Ye-Net, Yedroudj-Net, SR-Net, Zhu-Net, and GBRAS-Net with different image normalization.
- **SRM filters normalization** This folder contains the notebooks Xu-Net, Ye-Net, Yedroudj-Net, SR-Net, Zhu-Net, and GBRAS-Net with different image normalization, and SRM filters normalization.
- **Trained model** This folder contains the Ye-Net weights with WOW 0.4 bpp.

 
## Requirements
This repository requires the following libraries and frameworks:

- TensorFlow 
- numPy 
- OpenCV 
- Matplotlib
- Time
- random
- os
- scikit-image
- glob

This repository was developed in the Python3 (3.8) programming language.

## Package installation

if you don't use google colab, We highly recommend to use and install Python packages within an Anaconda enviroment. To create, execute the command below:
```
conda create --name Sensitivity python=3.8
```
So, activate it
```
conda activate Sensitivity 
```
installed the framework
```
conda install -c anaconda keras-gpu==2.4.3
```
Now, install the libraries.
```
pip install opencv-python
conda install -c conda-forge matplotlib
conda install -c jmcmurray os
conda install -c conda-forge time
conda install -c anaconda scikit-image
```
## Execution
After installing all the Requirements, you must clone the repository using.
```
git clone https://github.com/BioAITeam/Sensitivity-of-Deep-Learning-Applied-to-Spatial-Image-Steganalysis.git
```
If you will use colab, upload the cloned folder to drive, then open the folder of your choice and run either of the two notebooks.

if you are going to use your computer, install:
```
conda install jupyter 
```
Enter the cloned folder, hen open the folder of your choice and run either of the two notebooks.

## Note 
Before running the notebook, please verify that the file paths are correct.
## Databases


The data set used to reproduce the results can be downloaded from this <a href="https://drive.google.com/drive/folders/1G5vdhW11_qKfVC6W8_pfJpstVkXUk1QQ?usp=sharing">link</a>. Images taken from: <a href="http://agents.fel.cvut.cz/boss/index.php?mode=VIEW&tmpl=materials">BOSS competition</a> and <a href="http://bows2.ec-lille.fr/index.php?mode=VIEW&tmpl=index1">BOWS2</a>.
#### NPY
After accessing the link, enter the strategy folder 
#### PGM
After accessing the link, enter the GBRAS-Net folder 
