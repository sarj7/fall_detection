# Camera Based Activity Recognition for Assisted Living Applications

<div style="text-align: justify;">
Activity recognition in the assisted living environment can detect different dangerous and anomalous activities. One such activity is the act of falling, which is very dangerous and can cause injuries and death. According to a World Health Organization report [1], falling is the second leading cause of unintentional injury and death all over the world. About 684,000 people die due to falling worldwide. Approximately 37.3 million falls are severe enough to require medical attention each year. These metrics of falls are skewed, and populations aged 60 years and older experience the most number of falls. The unintentional deaths caused by falls can be prevented to a great extent by its early detection and providing subsequent medical help. Although several fall detection systems exist, they lack speed, and most of them are slow in terms of inference time.

We propose a single-shot fall detection model as part of camera-based activity recognition for assisted living applications, which is fast and accurate. The proposed fall detection model uses a deep learning-based object detection framework called YOLOv5. Instead of following a two-step process for fall detection, namely, subject of interest detection (object detection) and then activity recognition (fall activity recognition), we detect a fall in a single stage by virtue of object detection and activity recognition merged into a one-step process. This approach introduces novelty by using an object detection framework for activity recognition and fall detection. The proposed model is implemented in the PyTorch framework. We train different variants of YOLOv5 (small, medium, large) differentiated by their depth. The best result obtained shows an inference speed of 32 frames per second. This fall detection model detects falls accurately in challenging conditions with noise and background clutter. 

The subsequent qualitative examples presented here serve to demonstrate the effectiveness of our fall detection model, which is able to accurately identify instances of falling.
</div>

![result1](https://github.com/sarj7/fall_detection/blob/cd1623acd8dc371ec44c4696ec34342d0e4f7bc0/gifs/1.gif)

When subjected to unobserved instances of falling, our fall detection model demonstrated the capability to precisely identify the fall occurrence. 


![result2](https://github.com/sarj7/fall_detection/blob/cd1623acd8dc371ec44c4696ec34342d0e4f7bc0/gifs/2.gif)

An additional illustration in which our fall detection model aptly recognized a falling event.


![result3](https://github.com/sarj7/fall_detection/blob/cd1623acd8dc371ec44c4696ec34342d0e4f7bc0/gifs/s.gif)

During our experimentation, we assessed the efficacy of our fall detection model by applying it to a randomly selected YouTube video. The model accurately detected the occurrence of a fall event.
