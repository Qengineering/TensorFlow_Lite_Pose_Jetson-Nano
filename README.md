# TensorFlow_Lite_Pose_Jetson-Nano
![output image]( https://qengineering.eu/images/Pose_Jetson.webp )<br/>
## TensorFlow Lite Posenet running on a Jetson Nano
[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)<br/><br/>
A fast C++ implementation of TensorFlow Lite Posenet on a Jetson Nano.<br/>
Once overclocked to 2015 MHz, the app runs at 15.2 FPS.
Special made for a Jetson Nano see [Q-engineering deep learning examples](https://qengineering.eu/deep-learning-examples-on-raspberry-32-64-os.html) <br/>

------------

Papers: https://medium.com/tensorflow/real-time-human-pose-estimation-in-the-browser-with-tensorflow-js-7dd0bc881cd5<br/>

------------

## Benchmark.
| CPU 2015 MHz | GPU 2015 MHz | CPU 1479 MHz | GPU 1479 MHZ | RPi 4 64os 1950 MHz |
|  :------------: | :-------------: | :-------------:  | :-------------: | :-------------: |
|  15.2 FPS | 11.8 FPS  | 12 FPS | 11 FPS  | 9.4 FPS |

------------

## Dependencies.<br/>
To run the application, you have to:
- TensorFlow Lite framework installed. [Install TensorFlow Lite](https://qengineering.eu/install-tensorflow-2-lite-on-jetson-nano.html) <br/>
- Optional OpenCV installed. [Install OpenCV 4.5](https://qengineering.eu/install-opencv-4.5-on-jetson-nano.html) <br/>
- Code::Blocks installed. (```$ sudo apt-get install codeblocks```)

------------

## Installing the app.
To extract and run the network in Code::Blocks <br/>
$ mkdir *MyDir* <br/>
$ cd *MyDir* <br/>
$ wget https://github.com/Qengineering/TensorFlow_Lite_Pose_Jetson-Nano/archive/refs/heads/main.zip <br/>
$ unzip -j master.zip <br/>
Remove master.zip, LICENSE and README.md as they are no longer needed. <br/> 
$ rm master.zip <br/>
$ rm README.md <br/> <br/>
Your *MyDir* folder must now look like this: <br/> 
Dance.mp4 <br/>
posenet_mobilenet_v1_100_257x257_multi_kpt_stripped.tflite <br/>
TestTensorFlow_Lite_Pose.cpb <br/>
Pose_single.cpp<br/>

------------

## Running the app.
Run TestTensorFlow_Lite.cpb with Code::Blocks.<br/>
You may need to adapt the specified library locations in *TestTensorFlow_Lite.cpb* to match your directory structure.<br/><br/>
With the `#define GPU_DELEGATE` uncommented, the TensorFlow Lite will deploy GPU delegates, if you have, of course, the appropriate libraries compiled by bazel. [Install GPU delegates](https://qengineering.eu/install-tensorflow-2-lite-on-jetson-nano.html) <br/><br/>
See the RPi 4 movie at: https://www.youtube.com/watch?v=LxSR5JJRBoI

------------

[![paypal](https://qengineering.eu/images/TipJarSmall4.png)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=CPZTM5BB3FCYL) 


