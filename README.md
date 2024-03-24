# Safety Tracker: Enhancing Nighttime Security for Women

## Demo.mp4 has the demo video of how the proram works

This project introduces an advanced algorithm empowered by artificial intelligence, capable of dynamically detecting and tracking instances of potential stalking or harassment in real-time, even in low-light environments. Designed to enhance safety for women at night, it vigilantly monitors their surroundings, promptly alerting them to any looming dangers.

### Motivation
**Issue**: Women and young girls often experience street harassment, ranging from catcalls to assault.
**Existing Solutions**: Current safety apps have limited functionality, such as scream detection or manual activation by holding a button in the app
![image](https://github.com/amqsabnur/Safety-Tracking-with-artificial-intelligence/assets/36308612/884b74fd-1c0b-4067-b809-e5e272f6bad1)
**Proposal**: I aimed to develop a product that automatically detects threats, such as someone following you for an extended period.

## Diving into Technical Details
This safety tracking algorithm uses Computer Vision.
![image](https://github.com/amqsabnur/Safety-Tracking-with-artificial-intelligence/assets/36308612/61a2eb84-2bc5-4d9f-8f80-28475b44f348)

This Computer Vision algorithm combines YOLOv5 for real-time object detection and DeepSORT for object tracking.

YOLOv5: Real-time Object Detection:
  - YOLO (You Only Look Once) v5 is a state-of-the-art real-time object detection algorithm.
  - It employs a single neural network to predict bounding boxes and class probabilities directly from full images in one evaluation.
  - This allows for efficient and accurate detection of objects in real-time, crucial for identifying potential threats quickly.
  Architecture of the model is shown below:
![image](https://github.com/amqsabnur/Safety-Tracking-with-artificial-intelligence/assets/36308612/8c7d6254-8449-4e30-bda9-64f7c4f39285)


DeepSORT: Object tracking algorithm based on deep learning.
Utilized for tracking objects detected by YOLOv5 over time.
Slide 5: Methodology

Integration of YOLOv5 and DeepSORT for seamless real-time object detection and tracking.
Implementation details and challenges faced during development.
Slide 6: Results

Demonstration of the Third Eye system in action.
Evaluation metrics and performance analysis.
Slide 7: Application

Potential applications beyond nighttime security, such as surveillance systems, traffic monitoring, etc.
Impact on improving safety and security measures.
Slide 8: Conclusion

Summary of key findings and achievements.
Future directions and enhancements for the Third Eye project.
Slide 9: Q&A

Open floor for questions from the audience.
[Optional] Slide 10: Contact Information

Contact details for further inquiries or collaboration opportunities.
