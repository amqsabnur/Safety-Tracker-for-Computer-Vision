# Safety Tracker: Enhancing Nighttime Security for Women

This project introduces an advanced algorithm empowered by artificial intelligence, capable of dynamically detecting and tracking instances of potential stalking or harassment in real-time, even in low-light environments. Designed to enhance safety for women at night, it vigilantly monitors their surroundings, promptly alerting them to any looming dangers.

## Demo.mp4 has the demo video of how the tracker works
  - It draws a black box around a human when it detect that person for the first time
  - The black box becomes red when the person has been there for a long time
  - The black box also becomes red when a person detected previous dissapears and reappears in the user's surroundingß
![image](https://github.com/amqsabnur/Safety-Tracking-with-artificial-intelligence/assets/36308612/e2367768-e1e1-4557-a01e-3182bcb0bdb4)

### Motivation
**Issue**: Women and young girls often experience street harassment, ranging from catcalls to assault.
**Existing Solutions**: Current safety apps have limited functionality, such as scream detection or manual activation by holding a button in the app
![image](https://github.com/amqsabnur/Safety-Tracking-with-artificial-intelligence/assets/36308612/884b74fd-1c0b-4067-b809-e5e272f6bad1)
**Proposal**: I aimed to develop a product that automatically detects threats, such as someone following you for an extended period.

### Diving into Technical Details
This safety tracking algorithm uses Computer Vision.
![image](https://github.com/amqsabnur/Safety-Tracking-with-artificial-intelligence/assets/36308612/61a2eb84-2bc5-4d9f-8f80-28475b44f348)

This Computer Vision algorithm combines YOLOv5 for real-time object detection and DeepSORT for object tracking.

#### YOLOv5: Real-time Object Detection:
  - YOLO (You Only Look Once) v5 is a state-of-the-art real-time object detection algorithm.
  - It employs a single neural network to predict bounding boxes and class probabilities directly from full images in one evaluation.
  - This allows for efficient and accurate detection of unique objects in real-time, crucial for identifying potential threats quickly.

Architecture of the model is shown below:

![image](https://github.com/amqsabnur/Safety-Tracking-with-artificial-intelligence/assets/36308612/8c7d6254-8449-4e30-bda9-64f7c4f39285)


#### DeepSORT: Object tracking algorithm based on deep learning.
  - DeepSORT (Deep Learning for Object Tracking) is an advanced algorithm designed for tracking objects in video streams.
  - It utilizes deep learning techniques to associate object detections over multiple frames, enabling robust and accurate tracking of moving objects.
  - By combining YOLOv5's object detection with DeepSORT's tracking capabilities, the system can not only detect but also track potential threats, providing continuous surveillance and ensuring timely alerts in dynamic environments.

Architecture of the model is shown below:

![image](https://github.com/amqsabnur/Safety-Tracking-with-artificial-intelligence/assets/36308612/10850b30-6e63-4522-aa52-dc4b31d8efba)


#### Image Similarity
  - Next identify unique features in images and assign them numerical descriptions.
  - By comparing these descriptions between different images, you can track individuals over time, helping the slgorithm to spot any potential threats.

