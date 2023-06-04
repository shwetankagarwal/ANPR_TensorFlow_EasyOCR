# ANPR (Automatic Number Plate Recognition) using TensorFlow and EasyOCR

ANPR (Automatic Number Plate Recognition) is a project that utilizes TensorFlow and EasyOCR to recognize and extract license plate information from images or video frames. This project aims to provide an efficient and accurate solution for various applications, including traffic enforcement, toll collection, parking management, and vehicle tracking.

## Features

- License plate detection: Utilize TensorFlow to train a deep learning model to detect license plate regions within images or video frames.
- Character recognition: Train a separate model to recognize the characters within the detected license plate regions.
- EasyOCR integration: Integrate the trained TensorFlow models with EasyOCR library to extract and recognize the license plate numbers.
- High accuracy: EasyOCR offers a high accuracy rate in recognizing text from images, ensuring reliable license plate recognition results.

## Installation

<b>Step 1.</b> Clone this repository: https://github.com/shwetankagarwal/ANPR_TensorFlow_EasyOCR
<br/><br/>
<b>Step 2.</b> Create a new virtual environment 
<pre>
python -m venv anprsys
</pre> 
<br/>
<b>Step 3.</b> Activate your virtual environment
<pre>
source anprsys/bin/activate # Linux
.\anprsys\Scripts\activate # Windows 
</pre>
<br/>
<b>Step 4.</b> Install dependencies and add virtual environment to the Python Kernel
<pre>
python -m pip install --upgrade pip
pip install ipykernel
python -m ipykernel install --user --name=anprsys
</pre>
<br/>

## Usage

1. Prepare the dataset:
   - Collect a dataset of images or video frames containing license plates.
   - Annotate the dataset with license plate locations and corresponding text.

2. Data preprocessing:
   - Resize the images or video frames to a suitable input size for the ANPR model.
   - Normalize the pixel values of the images.
   - Prepare the annotations in a compatible format for training.

3. Training:
   - Train the license plate detection model using TensorFlow.
   - Train the character recognition model - EasyOCR.

4. Model evaluation:
   - Evaluate the trained models using a validation set to measure accuracy and performance.

5. Integration with EasyOCR:
   - Integrate the trained TensorFlow models with EasyOCR library.
   - Run the ANPR script to perform license plate recognition:

   The script will detect license plates in the image and provide the recognized license plate numbers.

## Contributing

Contributions are welcome! If you have any ideas or suggestions for improvement, please create an issue or submit a pull request.

## License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).

## Acknowledgements

- [TensorFlow](https://www.tensorflow.org/) - Open-source machine learning framework.
- [EasyOCR](https://github.com/JaidedAI/EasyOCR) - Python library for Optical Character Recognition.
