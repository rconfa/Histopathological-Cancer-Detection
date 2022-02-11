<p float="left">

 <img src="https://github.com/rconfa/Histopathological-Cancer-Detection/blob/main/images/DSLogo.png" width = "500"/>
 <img src="https://github.com/rconfa/Histopathological-Cancer-Detection/blob/main/images/BicoccaLogo.png" width = "100" align="right"/>
</p>
<h2 align="center">Advanced Machine Learning project</h2>

# Histopathological-Cancer-Detection
Created an algorithm to identify metastatic cancer in small image patches taken from larger digital pathology scans. The data used for this competition is a slightly modified version of the PatchCamelyon (PCam) benchmark dataset. The original PCam dataset contains duplicate images due to its probabilistic sampling, however, the version presented on Kaggle does not contain duplicates.

# Motivation 

# Data
The data are taken from a Kaggle challenge published in 2018 and they can be downloaded [here](https://www.kaggle.com/c/histopathologic-cancer-detection/data). For the project two subset has been created in order to speed up the learning process and create nested folder for appropriately using keras import method. Due to their size it is impossible to upload them in Github but feel free to contact me if you need them. <br>
The original dataset has more than 220K RGB images with a dimension of 96x96x3. The given problem is the binary classification problem where the associated label has two class labels i.e. tumor and non-tumor tissues. A positive label indicates that the center 32x32px region of a patch contains at least one pixel of tumor tissue. No information is given for the outside region.

# Notebook 

* [<b>1_ResizingTrainingData</b>](https://github.com/rconfa/Histopathological-Cancer-Detection/blob/main/Notebook/1_ResizingTrainingData.ipynb): load the data and creates a balanced subset of them. You can set the desidered size by changing the parameter `n_samples`. Moreover the data will be saved in different folder for splitting tumor and non-tumor images.
* [<b>2_HistopathologicCancerDetection_FineTuning</b>](https://github.com/rconfa/Histopathological-Cancer-Detection/blob/main/Notebook/2_HistopathologicCancerDetection_FineTuning.ipynb): contains the developed code for three different fine-tuning architecture (VGG16, DenseNet-201, MobileNet-V2. It also contains the tuning of the related hyperparameters.
* [<b>3_HistopathologicCancerDetection_ModelFromScratch</b>](https://github.com/rconfa/Histopathological-Cancer-Detection/blob/main/Notebook/3_HistopathologicCancerDetection_ModelFromScratch.ipynb): contains the developed code for a convolutional neural network from scratch. Contains several versions of this CNN and hyperparameter optimization. 

# Results Table


# References
[1] V. Messina and S. Bianco, “Dispense e slide del corso advanced machine learning,” 2021. <br>
[2] PCCam, “Histopathologic cancer detection,” 2019. <br>
[3] K.-S. Lee, S.-H. Son, S.-H. Park, and E. Kim, “Automated detection of colorectal tumors based on artificial intelligence”. <br>
[4] PCCam, “Histopathologic cancer detection,” 2019. [Online]. Available: https://www.kaggle.com/c/histopathologic-cancer-detection/data. 


# About us

#### Riccardo Confalonieri - Data Science Student @ University of Milano-Bicocca
  * r.confalonieri5@campus.unimib.it
  * [GitHub](https://github.com/rconfa)
  * [LinkedIn](https://www.linkedin.com/in/riccardo-confalonieri-5250b0201/)

#### Cogo Luca - Data Science Student @ University of Milano-Bicocca
  * l.cogo@campus.unimib.it
  * [GitHub](https://github.com/LucaCogo)
  * [LinkedIn](https://www.linkedin.com/in/luca-cogo)

