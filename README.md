<div align="center">

# Spyder_RC_Car_TF_Model

</div>


<p align="center">
  <img src="https://github.com/AydenBravender/Spyder_RC_Car_TF_Model/blob/main/WIN_20230822_17_01_26_Pro.jpg" alt="Example of image model was trained on" width="65%" height="65%">>
</p>

## Overview
This model is based on the 'ssd-mobilenet-v2-fpnlite-320' architecture and was trained as a TensorFlow Lite model. The training dataset consisted of over 300 annotated images, covering a range of objects and backgrounds. The annotations were created using LabelImg. The model was fine-tuned using the approach outlined in the excellent guide by [Edje Electronics](https://github.com/EdjeElectronics/TensorFlow-Lite-Object-Detection-on-Android-and-Raspberry-Pi). The object detection model was trained on one class ```Car``` and is used to identify the above image type of RC cars. On the Raspberry Pi 4, it had a Fps of 4 frames per second.

## Running it on Raspberry Pi 4
To run the model, I followed Edje Electronics guide. You can either go to his guide and follow his steps, or follow the ones listed here.

First udpate/upgrade your computer by typing this into your terminal: ```sudo apt-get update``` and ```sudo apt-get upgrade```. 

Make sure that camera is enabled on your raspberry pi. Then clone ```git clone https://github.com/EdjeElectronics/Tensorflow-Lite-Object-Detection-on-Android-and-Raspberry-Pi.git```. 

Optional: I would rename the folder something simpler like TFlite1, as suggested by Edje Electronics. 

Next we use ```cd tflite1``` to work within the folder. Install virtualenv by ```sudo pip3 install virtualenv```. 

Run ```python3 -m venv tflite1-env``` and ```source tflite1-env/bin/activate```. 

Next run ```bash_get_pi_requirements.sh```. Move the Custom_model_lite file into your tflite1 folder. 

Finally run ```python3 TFlite_detection_webcam.py --modeldir=Custom_model_lite```. This should run the program on either a pi camera or a usb camera.

### Acknowledgments
This project would not be possible without the indepth tutorial by [Edje Electronics](https://github.com/EdjeElectronics/TensorFlow-Lite-Object-Detection-on-Android-and-Raspberry-Pi).

