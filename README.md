# Traffic Sign Display on Car Windshield

## Motivation

Automobile accidents remain a leading cause of injuries and fatalities globally, with India experiencing a significant share of this burden. According to the report *Distracted Driving in India: A Study on Mobile Phone Usage, Pattern & Behaviour*, India accounts for over 10% of global road crash fatalities despite having only 1% of the world's vehicles. Key statistics include:

- A road crash occurs every minute, with a fatality every four minutes.
- 47% of drivers receive calls while driving, and 60% do not stop safely to answer them.
- 96% of passengers feel unsafe when drivers are distracted.

This project addresses these issues by notifying drivers about road signs directly on the windshield, alleviating the pressure of scanning roadsides and improving focus on driving.

## Objectives

The primary goals of this project are:

1. To reduce the risk associated with driving by making road sign information easily accessible without diverting attention.
2. To decrease car accidents by at least 1%, considering even a small reduction as a significant achievement.
3. To leverage technology to enhance human life by making driving safer and less stressful.

## Hypothesis

The system hypothesizes that a Pi camera can capture road sign images, process them using a pre-trained dataset of road signs, and project corresponding messages onto the car's HUD. This enables drivers to maintain focus on the road while staying informed about traffic signs.

## Methodology

The project employs the following workflow:

1. **Image Capture**: A Pi camera captures images of road signs.
2. **Image Processing**: The captured image is processed using OpenCV for enhancement and preparation.
3. **Image Detection**: YOLOv5 (You Only Look Once, version 5) detects and identifies the road sign by comparing it against a dataset from Roboflow.
4. **Prediction**: The system predicts the most probable road sign based on trained data.
5. **Display**: The relevant message is projected onto the car's Heads-Up Display, allowing the driver to read it without looking away.

## Tools and Technologies

- **Python Libraries**:
  - **OpenCV**: For image processing.
  - **YOLOv5**: For object detection and training.
  - **PyTorch**: As the framework for running YOLOv5 models.
  - **Roboflow Dataset**: Provides a comprehensive set of road sign images for training and prediction.
- **Hardware**: Pi camera interfaced with the system for real-time image capture.

## Novelty

This project is an interdisciplinary effort combining computer science and engineering principles. It integrates:

- YOLOv5 for cutting-edge object detection.
- OpenCV for robust image processing.
- Roboflow dataset for reliable training data.
- PyTorch for efficient model execution.

This fusion creates a practical solution tailored to improve road safety.

## Analytical Insights

The project draws inspiration from alarming statistics:

- India lost 1.3 million lives to road crashes in the last decade, with 5.3 million seriously injured.
- 99% of people recognize mobile phone use while driving as dangerous, yet distractions persist.
- 41% of drivers use phones for work-related purposes, increasing risk.

By reducing distractions caused by roadside sign observation, this system aims to mitigate such risks.

## Installation and Setup

### Prerequisites

- Python 3.x
- Raspberry Pi with Pi Camera (optional for hardware implementation)
- A compatible Heads-Up Display unit (for real-world deployment)

### Hardware Setup

Below is an image of the hardware setup used in this project:

![image](https://github.com/user-attachments/assets/fa79ab8d-05fb-4379-90e6-149ec9e1ef61)


*The setup includes a Raspberry Pi with a Pi Camera mounted on the car's dashboard, connected to a Heads-Up Display (HUD) unit for projecting traffic sign information onto the windshield.*

## Output

Below is an example of the output displayed on the car's Heads-Up Display (HUD):

![image](https://github.com/user-attachments/assets/4f285be8-1d2e-4894-9782-2ef37a319a26)

