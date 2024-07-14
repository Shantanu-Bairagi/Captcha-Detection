CAPTCHA Detection
Table of Contents
Overview
Objectives
Dataset
Pre-processing
Methodology
Results
Dependencies
Usage
Contributing
License
Overview
This project focuses on developing a classification model to predict whether a given hexadecimal CAPTCHA is even or odd. The solution involves image pre-processing, augmentation, and digit detection techniques to achieve high accuracy and efficiency.

Objectives
Learn and develop a classification model for predicting the parity (even/odd) of hexadecimal CAPTCHAs.
Pre-process the CAPTCHA images by converting them to grayscale, applying binary thresholding, and removing stray lines using dilation.
Develop a method to detect the last digit using an image augmentation technique on a reference digit dataset.
Achieve a high parity score with minimal processing time.
Dataset
The dataset consists of hexadecimal CAPTCHA images. A reference digit dataset is used for image augmentation and last digit detection.

Pre-processing
Convert the image to grayscale.
Apply binary thresholding to highlight the digits.
Use dilation to remove stray lines and noise from the image.
Methodology
Image Pre-processing:

Convert images to grayscale.
Apply binary thresholding.
Use dilation to clean up the images.
Digit Detection:

Utilize an image augmentation technique on a reference digit dataset to detect the last digit of the CAPTCHA.
Classification:

Predict whether the CAPTCHA is even or odd based on the detected last digit.
Results
Achieved a parity score of 1.0 on the dataset.
Processing time: 0.007 seconds per image.
Dependencies
Python 3.x
OpenCV
NumPy
Matplotlib
Concurrent Futures (for parallel processing)
Install the dependencies using:

sh
Copy code
pip install opencv-python-headless numpy matplotlib
Usage
Clone the repository:
sh
Copy code
git clone https://github.com/yourusername/captcha-detection.git
cd captcha-detection
Ensure the dataset and reference images are in the correct directories.

Run the main script:

sh
Copy code
python main.py
Contributing
Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

License
This project is licensed under the MIT License - see the LICENSE file for details.
