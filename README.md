## Ship Detection in SAR Images using YOLOv7 and Noise Reduction

### Project Overview

This repository presents a ship detection model built upon the YOLOv7 architecture. To enhance the performance of the model, we've incorporated a preprocessing pipeline involving DDPM and anisotropic diffusion to mitigate noise prevalent in SAR images. The model is trained on a combination of SSDD, DS SDD, and Fusar datasets. 

**Key Components**

* **Noise Reduction:** DDPM and anisotropic diffusion are employed to preprocess SAR images, significantly reducing noise and improving image quality.
* **Object Detection:** YOLOv7 serves as the backbone for detecting ships within the preprocessed images, providing accurate bounding boxes and confidence scores.
* **Dataset:** The model is trained on a merged dataset comprised of SSDD, DS SDD, and Fusar, ensuring robustness and diversity in ship appearance.


**Future Work**

* Explore different noise reduction techniques (e.g., wavelet denoising)
* Incorporate additional datasets for increased model diversity
* Optimize YOLOv7 architecture for SAR image processing

**Contribution**

We welcome contributions to this project. Please feel free to submit pull requests with improvements or bug fixes.
