<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/bkctrl/gesture-detector">
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/2/2d/Tensorflow_logo.svg/1200px-Tensorflow_logo.svg.png" alt="Logo" width="80" height="80">
  </a>

<h3 align="center">Gesture Detector</h3>

  <p align="center">
  A ML-driven gesture detector web app that detects and classifies different hand gestures.    <br/><br/>
    <a href="https://www.gesturedetector.live"><strong>View Demo »</strong></a>
    <br />
    <br />
  </p>
</div>

<h2 align="center">Try these gestures</h2>


<!-- ABOUT THE PROJECT -->
## About The Project

[![Product Name Screen Shot][product-screenshot]](https://example.com)

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent vitae dictum lorem. Proin dui enim, efficitur sit amet hendrerit non, rutrum dapibus diam. Suspendisse potenti. Nulla facilisi. 

<p align="right">(<a href="#readme-top">back to top</a>)</p>

</table>


### Built With
<a href=""><img src="https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54"></a>
<a href=""><img src="https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white"></a>
<a href=""><img src="https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white" alt="X11"></a>
<a href=""><img src="https://img.shields.io/badge/opencv-%23white.svg?style=for-the-badge&logo=opencv&logoColor=white"></a>
<a href=""><img src="https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB" alt="X11"></a>
<a href=""><img src="https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E" alt="X11"></a>
<p align="right">(<a href="#readme-top">back to top</a>)</p>


## Getting Started

1. Create a new Python virtual environment.
```
python -m venv [venv-name]
```

2. Activate the environment.<br>
Linux/MacOS:
```
source [venv-name]/bin/activate
```
Windows:
```
.\[venv-name]\Scripts\activate # Windows
```

3.  Update pip and install ipykernel.
```
python -m pip install --upgrade pip
pip install ipykernel
python -m ipykernel install --user --name=[venv-name]
```

4. Using `image_collection.ipynb`, collect images with the window opened with OpenCV. 


5. Generate annotations of the collected images.


6. Divide collected images and annotations into `train` and `test` subfolders. The images and annotations in the `train` folder would be trained and the result will be compared to the the expected performance on the files in the `test` folder. 


7. Train the model with `train_detection.ipynb`. You may adjust the TensorFlow Zoo model being used (https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/tf2_detection_zoo.md) as desired. 

8. Export the model into TensorflowJS-format, included in `train_detection.ipynb`. Files `model.json`, `group1-shard1of3.bin`, `group1-shard2of3.bin`, and `group1-shard3of3.bin` should be generated. Keep this for future use.

9. Install dependencies for the web-app implementation.
```
npm install
```

10. Copy `model.json`, `group1-shard1of3.bin`, `group1-shard2of3.bin`, and `group1-shard3of3.bin` from above into the `web/public` directory. 

11. Start the app!
```
npm start
```
