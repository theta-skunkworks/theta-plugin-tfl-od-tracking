# Object tracking sample using TF-Lite Object Detection and equirectangular rotation processing

より詳しい日本語の説明は[こちら](https://qiita.com/KA-2/未定)。<br>
[Click here](https://qiita.com/KA-2/未定) for a more detailed explanation in Japanese.


このソフトウェアは、 Apache 2.0ライセンスで配布されている製作物が含まれています。<br>
This software includes the work that is distributed in the Apache License 2.0.


## Overview

This is a sample program that tracks bananas recognized using Object Detection of TensorFlow Lite in all directions.
It includes the following technical elements:

- How to use TensorFlow Lite Object Detection
- Equirectangular rotation process written using NDK's OpenCV
- Use of THETA posture information


![OmnidirectionalTracking](img/OmnidirectionalTracking.gif)


## Build

To build this set of project files, you need to do the following three things yourself.

### Download and deploy [OpenCV Android pack 3.4.9](https://sourceforge.net/projects/opencvlibrary/files/3.4.9/opencv-3.4.9-android-sdk.zip/download)

The example of the deployment destination is as follows

```
C:/opencv/OpenCV-3.4.9-android-sdk
```

Please rewrite the "Path to OpenCV.mk" described in Android.mk according to the result of expanding the file.



### Android Studio settings (setting to enable NDK build)


Open "Tools"-> "SDK Manager"-> "SDK Tools" and make sure the following items are checked.


- Android SDK Build-Tools
- Android SDK Platform-Tools
- Android SDK Tools
- Google USB Driver
- NDK
 
### Download and install "[Java SE Development Kit 8](https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)"


###  Copy of OpenCV library (.so file)

```
Source     : C:/(The location of OpenCV Android pack)/sdk/native/libs/arm64-v8a
Destination: C:/(The location of the project file)/app/jniLibs/arm64-v8a
```



## Development Environment

### Camera
* RICOH THETA V Firmware ver.3.30.1 and above
* RICOH THETA Z1 Firmware ver.1.40.1 and above

### SDK/Library
* RICOH THETA Plug-in SDK ver.2.0.10

### OpenCV Android pack
* opencv-3.4.9-android-sdk

### TensorFlow Lite Object Detection model
* coco_ssd_mobilenet_v1_1.0_quant_2018_06_29.zip

### Development Software
* Android Studio ver.3.5.3
* gradle ver.5.1.1


## License

```
Copyright 2018 Ricoh Company, Ltd.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```

## Contact
![Contact](img/contact.png)

