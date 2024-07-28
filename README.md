## Ship Detection in SAR Images using YOLOv7 and Noise Reduction

### Project Overview

This repository presents a ship detection model built upon the YOLOv7 architecture. To enhance the performance of the model, we've incorporated a preprocessing pipeline involving DDPM and anisotropic diffusion to mitigate noise prevalent in SAR images. The model is trained on a combination of SSDD, DS SDD, and Fusar datasets. 

**Key Components**

* **Noise Reduction:** DDPM and anisotropic diffusion are employed to preprocess SAR images, significantly reducing noise and improving image quality.
* **Object Detection:** YOLOv7 serves as the backbone for detecting ships within the preprocessed images, providing accurate bounding boxes and confidence scores.
* **Dataset:** The model is trained on a merged dataset comprised of SSDD, DS SDD, and Fusar, ensuring robustness and diversity in ship appearance.

**Getting Started**

1. **Environment Setup:**
    * Install required dependencies (list specific dependencies)
    * Clone this repository: `git clone https://github.com/<your-username>/ship-detection-sar`
2. **Download Datasets:**
    * Download the SSDD, DS SDD, and Fusar datasets (provide download instructions or links)
    * Unzip the datasets and place them in the `data` folder
3. **Training the Model:**
    * Run the training script: `python train.py`
    * (Optional) Modify training hyperparameters in `config.py`
4. **Evaluation:**
    * Run the evaluation script: `python evaluate.py`
    * This script will output metrics such as mAP, precision, recall, and F1-score

**Results**

[Present evaluation metrics, such as mAP, precision, recall, and F1-score in a clear table or visualization]

**Future Work**

* Explore different noise reduction techniques (e.g., wavelet denoising)
* Incorporate additional datasets for increased model diversity
* Optimize YOLOv7 architecture for SAR image processing

**License**

[Specify the license used for your project (e.g., MIT, Apache 2.0)]

**Contribution**

We welcome contributions to this project. Please feel free to submit pull requests with improvements or bug fixes.
