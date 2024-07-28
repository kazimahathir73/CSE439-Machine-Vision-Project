Ship Detection in SAR Images using YOLOv7
This repository contains the code and resources for our project on detecting ships from Synthetic Aperture Radar (SAR) images using the YOLOv7 model. We have trained the model on various datasets, including SSDD, DS SDD, and FUSAR, and implemented techniques such as Denoising Diffusion Probabilistic Models (DDPM) and anisotropic diffusion to reduce noise in the images before training.

Table of Contents
Introduction
Datasets
Preprocessing
Model Training
Results
Installation
Usage
Contributing
License
Introduction
In this project, we focus on detecting ships from SAR images using the YOLOv7 model. SAR images often contain a significant amount of noise, which can hinder the performance of object detection models. To address this, we apply noise reduction techniques such as Denoising Diffusion Probabilistic Models (DDPM) and anisotropic diffusion before training our model.

Datasets
We have used the following datasets for training and testing:

SSDD (SAR Ship Detection Dataset)
DS SDD (Deep Sea Ship Detection Dataset)
FUSAR (Fusion SAR Dataset)
Preprocessing
To enhance the quality of SAR images and reduce noise, we implemented the following preprocessing steps:

Denoising Diffusion Probabilistic Models (DDPM): Applied to remove noise while preserving important features of the images.
Anisotropic Diffusion: Used to further smooth the images and reduce noise.
Model Training
The preprocessed images were then used to train the YOLOv7 model. YOLOv7, known for its efficiency and accuracy in object detection, was fine-tuned on our datasets to detect ships accurately in SAR images.

Results
The trained model demonstrated high accuracy in detecting ships in SAR images, with significant improvements observed due to the noise reduction techniques employed.

Installation
To set up the project locally, follow these steps:

Clone the repository:

bash
Copy code
git clone https://github.com/yourusername/ship-detection-yolov7.git
cd ship-detection-yolov7
Install the required dependencies:

bash
Copy code
pip install -r requirements.txt
Download the datasets and place them in the data/ directory.

Usage
To run the model on a new set of SAR images, use the following command:

bash
Copy code
python detect.py --source path_to_images --weights yolov7_weights.pth
For detailed usage instructions, refer to the documentation in the docs/ folder.

Contributing
We welcome contributions to this project. If you have any suggestions or improvements, please open an issue or submit a pull request.
