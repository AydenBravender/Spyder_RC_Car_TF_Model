<div align="center">

# Spyder_RC_Car_TF_Model

</div>


<p align="center">
  <img src="https://github.com/AydenBravender/Spyder_RC_Car_TF_Model/blob/main/WIN_20230822_17_01_26_Pro.jpg" alt="Example of image model was trained on" width="65%" height="65%">>
</p>

## Overview
This model is based on the 'ssd-mobilenet-v2-fpnlite-320' architecture and was trained as a TensorFlow Lite model. The training dataset consisted of over 300 annotated images, covering a range of objects and backgrounds. The annotations were created using LabelImg. The model was fine-tuned using the approach outlined in the excellent guide by [Edje Electronics](https://github.com/EdjeElectronics/TensorFlow-Lite-Object-Detection-on-Android-and-Raspberry-Pi). It's worth noting that fine-tuning was employed rather than starting from scratch. The object detection model was trained on one class ```Car``` and is used to identify the above image type of RC cars. On the Raspberry Pi 4, it had a Fps of 4 frames per second.

### Acknowledgments
This project would not be possible without the indepth tutorial by [Edje Electronics](https://github.com/EdjeElectronics/TensorFlow-Lite-Object-Detection-on-Android-and-Raspberry-Pi).

