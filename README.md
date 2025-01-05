AI-Driven Electrochemical Image Generation and Classification<br>
This repository contains two parts of the software used in the research paper "Artificial Intelligence-assisted electrochemical sensors for qualitative and semi-quantitative multiplexed analyses". The software pipeline is split into two main components:<br>
<br>
Java Module: Responsible for generating images from voltammetric data.<br>
Python Module: This module is used to classify the generated images and identify pollutants.<br>

Prerequisites<br>
Java 21 or higher<br>
Python 3.12 or higher<br>

Required Python libraries listed in requirements.txt<br>
<br>
Structure<br>
java/: Contains the Java code for generating images from voltammetric sequences.<br>
python/: Contains the Python code for image classification using machine learning models.<br>
data/: Folder where input voltammetric data and generated images are stored.<br>
<br>
Java Module: Image Generation<br>
The Java module converts voltammetric data into images using Gramian Angular Field (GAF) transformations. These images serve as input for the classification module. To run the Java module, navigate to the java/ directory and execute the following command:<br>
<br>
gaf_generation.sh<br>
Output images will be saved in the data/images/ folder.<br>
<br>
Python Module: Image Classification<br>
The Python module uses a Convolutional Neural Network (CNN) to classify the images generated from the voltammetric sequences. The classification is based on identifying the presence of specific pollutants in the sample.<br>
<br>
To set up the Python environment, run:<br>
<br>
pip install -r requirements.txt<br>
Then, to run the classification:<br>
<br>
gaf_cnn.sh<br>
The results will be shown on the screen, including classification accuracy and pollutant identification.<br>
<br>
Dataset<br>
The dataset used for training and validation consists of voltammetric sequences transformed into images. The images are stored in the data/ folder and classified according to the pollutants detected.<br>
<br>
Citation<br>
If you use this software for your research, please cite our paper:<br>
<br>
Rocco Cancelliere, Mario Molinara, Antonio Maffucci, Laura Micheli, "Artificial Intelligence-assisted electrochemical sensors for qualitative and semi-quantitative multiplexed analyses."<br>
