AI-Driven Electrochemical Image Generation and Classification
This repository contains two parts of the software used in the research paper "Artificial Intelligence-assisted electrochemical sensors for qualitative and semi-quantitative multiplexed analyses". The software pipeline is split into two main components:

Java Module: Responsible for generating images from voltammetric data.
Python Module: Used for classifying the generated images to identify pollutants.

Prerequisites
Java 21 or higher
Python 3.12 or higher

Required Python libraries listed in requirements.txt

Structure
java/: Contains the Java code for generating images from voltammetric sequences.
python/: Contains the Python code for image classification using machine learning models.
data/: Folder where input voltammetric data and generated images are stored.

Java Module: Image Generation
The Java module converts voltammetric data into images using Gramian Angular Field (GAF) transformations. These images serve as input for the classification module. To run the Java module, navigate to the java/ directory and execute the following command:

java Main path/to/voltammetric/data
Output images will be saved in the data/images/ folder.

Python Module: Image Classification
The Python module uses a Convolutional Neural Network (CNN) to classify the images generated from the voltammetric sequences. The classification is based on identifying the presence of specific pollutants in the sample.

To set up the Python environment, run:

pip install -r requirements.txt
Then, to run the classification:

python classifier.py path/to/images
The results, including classification accuracy and pollutant identification, will be saved in the results/ folder.

Dataset
The dataset used for training and validation consists of voltammetric sequences transformed into images. The images are stored in the data/ folder and classified according to the pollutants detected.

Citation
If you use this software for your research, please cite our paper:

Rocco Cancelliere, Mario Molinara, Antonio Maffucci, Laura Micheli, "Artificial Intelligence-assisted electrochemical sensors for qualitative and semi-quantitative multiplexed analyses."
