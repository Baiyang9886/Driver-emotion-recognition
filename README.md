A Robust Driver Emotion Recognition Method Based on High-Purity Feature Separation
====

Since emotions generally affect driver's behavior, judgment, and reaction time, accurately identifying driver's emotions is of great significance to improve the safety and comfort of intelligent driving system. However, the gender, skin color, age, and appearance of different drivers often have big differences, which will greatly interfere with the emotional recognition process. Besides, light intensity inside the vehicle varies with different time, weather, and location, which will also pose a challenge to driver emotion recognition. In this paper, a robust driver emotion recognition method based on feature separation is proposed to overcome the interference of individual differences and illumination changes. In order to realize the separation of expression-related features and irrelevant features, we design a high-purity feature separation (HPFS) framework based on partial feature exchange and the constraints of multiple loss functions. Moreover, we create a multiple light intensities driver emotion recognition (MLI-DER) dataset and conduct a great deal of experiments on the dataset to verify that  our method can overcome the interference of illumination changes. In addition, some cross-subject emotion recognition experiments are conducted on two public facial expression recognition dataset FACES and Oulu-CASIA to further demonstrate that our method can largely alleviate the interference of individual difference by comparing the experimental results with that of some state-of-the-art methods.

Multiple light intensities driver emotion recognition (MLI-DER) dataset
-------

<div align="center">
  
| Data acquisition system | Representative samples |
| ---------- | -----------|
| ![Image](https://github.com/Baiyang9886/Driver-emotion-recognition/blob/main/setup.jpg) | ![Image](https://github.com/Baiyang9886/Driver-emotion-recognition/blob/main/sample.jpg)  |
| Fig. 1 The data acquisition system of the MLI-DER dataset. | Fig. 2 Sample presentation of the MLI-DER dataset.  |

</div>

To verify that the proposed driver emotion recognition method can adapt to different light conditions, the MLI-DER dataset is created in this paper. The data acquisition system is shown in Fig. 1, which consists of a set of simulated driving system (Logitech G29), a computer, a camera (Logitech C920 Pro), and data record equipment. In the data collection process, each subject drives a car through the simulated driving system and performs three categories of expressions (negative, neutral, positive) according to the prompts. The camera facing experimental subjects will record the facial video data of drivers during the whole driving process. In addition, we create four scenes with different light intensities (dark, normal, little bright, and very bright) by controlling the light of the laboratory, and a set of data for each subject under the four light intensities are collected, respectively, some instances are shown in Fig. 2. In the process of data processing, we clip the collected videos into video samples according to positive expression, neutral expression, and negative expression. In this paper, we invite 37 subjects (12 female and 25 male) with ages ranging from 21 to 37 and obtain 442 video samples in total after the clipping process. The frame rate and resolution of each video are 20 fps and 640 X 480 pixels. In the experiments of this paper, the keyframes are captured from each video, and a total of 4451 image samples are obtained finally.

![Image](https://github.com/Baiyang9886/Driver-emotion-recognition/blob/main/sample.jpg)
Fig. 2 Sample presentation of the MLI-DER dataset. In the figure, the four columns of samples are collected under the light intensity of dark, normal, little bright and very bright, respectively. In addition, the first row is image with neutral expression, the second row is image with negative expression, and the third row is image with positive expression.

### Dataset download link
The MLI-DER dataset has been publicly released to all researchers of the relevant fields. The download link for the dataset is: https://drive.google.com/drive/folders/1iDa5qV8viq-MjnlWqeQkJdTJEB576YCr?usp=drive_link
