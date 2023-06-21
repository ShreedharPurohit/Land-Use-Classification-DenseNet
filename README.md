# Land Use Scene Classification using DenseNet

This repository contains code for performing land use scene classification using the DenseNet model in Python. The project aims to classify images into 21 different land use classes, including agricultural, airplane, baseballdiamond, beach, buildings, chaparral, denseresidential, forest, freeway, golfcourse, harbor, intersection, mediumreesidential, mobilehomepark, overpass, parkinglot, river, runway, sparseresidential, storagetanks, and tenniscourt.

## Table of Contents

- [Features](#features)
- [Dataset](#dataset)
- [Requirements](#requirements)
- [Usage](#usage)
- [Results](#results)
- [Credits](#credits)
- [Contributing](#contributing)
- [Contact](#contact)

## Features

- Utilizes the DenseNet121 pre-trained model for feature extraction.
- Fine-tunes the model on the land use scene classification task using transfer learning.
- Implements data augmentation techniques such as image shearing, zooming, and flipping for better model generalization.
- Evaluates the model's performance using metrics like accuracy, F1 score, precision, and recall.
- Provides a graphical representation of the F1 score for each class.

## Dataset

The dataset used for training, testing, and validation is organized into separate directories for each set. The directory structure should be as follows:

__images_train_test_val/__

__train/__

class1/

img1.jpg

img2.jpg

...

class2/

img1.jpg

img2.jpg

...

...

__test/__

class1/

img1.jpg

img2.jpg

...

class2/

img1.jpg

img2.jpg

...

...

__validation/__

class1/

img1.jpg

img2.jpg

...

class2/

img1.jpg

img2.jpg

...

...


Ensure that the directory paths for train, test, and validation sets are correctly specified in the code.

## Requirements

- Python 3.x
- TensorFlow 2.x
- Keras
- NumPy
- Matplotlib
- scikit-learn

Install the required dependencies by running the following command:

```shell
pip install tensorflow numpy scikit-learn keras matplotlib
```

## Usage

- Place your dataset in the appropriate directory structure as mentioned above.
- Modify the code to set the correct directory paths, image size, batch size, and other parameters if required.
- Run the Python script to train the model on the dataset.
- After training, the model is saved as DenseNet.h5.
- To evaluate the model and generate predictions, run the Python script for prediction after modifying it with the correct file paths.
- The classification report, F1 score, precision, and recall will be printed to the console.
- Additionally, a bar graph showing the F1 score for each class will be displayed.
- Feel free to experiment with different parameters, network architectures, or extend the code to suit your requirements.

## Results

The performance of the land use scene classification model is evaluated using various metrics.

The classification report provides detailed metrics such as precision, recall, F1 score, and support for each class. 

Additionally, a bar graph is generated to visualize the F1 score for each class.

## Credits

The DenseNet model is used from the TensorFlow Keras library.

The dataset used for land use scene classification is obtained from __https://www.kaggle.com/datasets/apollo2506/landuse-scene-classification__.

## Contributing

  Contributions are welcome! If you find any issues or have suggestions for improvement, please submit a pull request or open an issue.

## Contact

  If you have any questions or inquiries, please feel free to contact [Shreedhar Purohit] at [shreedhar2.purohit@gmail.com].
