# Black and White Image Colorization with Deep Learning

This project demonstrates the colorization of black and white images using OpenCV and a pre-trained deep learning model. The model used is based on a Caffe implementation and provides a powerful example of how deep learning can be applied to computer vision tasks.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Setup and Installation](#setup-and-installation)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## Introduction

Colorizing black and white images involves using a deep learning model to predict the color information (chrominance) based on the grayscale information (luminance). This project uses a pre-trained model provided by Richard Zhang et al. and implements the colorization pipeline using Python and OpenCV.

## Features

- Load and preprocess black and white images
- Use a pre-trained Caffe model to predict color information
- Post-process and combine model outputs with original luminance to produce colorized images
- Display original and colorized images side by side

## Technologies Used

- Python
- OpenCV
- Caffe
- Numpy

## Setup and Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/yourusername/colorizeML.git
   cd colorizeML

2. **Download Pre-trained Model and Files**

   - [colorization_deploy_v2.prototxt](https://github.com/richzhang/colorization/tree/caffe/colorization/models)
   - [colorization_release_v2.caffemodel](https://github.com/richzhang/colorization/blob/caffe/colorization/resources/pts_in_hull.npy)
   - [pts_in_hull.npy](https://www.dropbox.com/s/dx0qvhhp5hbcx7z/colorization_release_v2.caffemodel?dl=1)

3. **Organize the Files and Folders**
   
     - Put all these three files into the folder named "model".
     - Put colorize.py file outside the model folder.
     - Make a folder "images" and store all black & white images there.
  
3. **Install Dependencies**

   Make sure you have Python installed, then install the required packages:

   ```bash
   pip install numpy opencv-python argparse

## Usage

1. **Run the Script**

   To colorize a black and white image, use the following command:

   ```bash
   python colorize.py --image images/filename.jpg

 Replace path/to/your/image.jpg with the path to your black and white image.

2. **Viewing Results**

   The script will display the original black and white image alongside the colorized version.

## Results

 Here are some example results of the colorization process:

 ![Black & white to colored image](https://github.com/mohdamaan069/b-w_Image_Colorization/blob/main/imge.png)


 # Contributing

Contributions are welcome! If you have any suggestions or improvements, feel free to create a pull request or open an issue.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

- The pre-trained model and weights are provided by Richard Zhang et al.
- This project is inspired by the work done in the paper ["Colorful Image Colorization"](https://arxiv.org/abs/1603.08511) by Richard Zhang, Phillip Isola, and Alexei A. Efros.

