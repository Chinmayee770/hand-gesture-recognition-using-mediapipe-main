# Hand Gesture Controlled Wheelchair

## Problem Statement
People with mobility impairments often face challenges in navigating their surroundings using traditional wheelchairs. Many individuals with conditions such as paralysis, muscular dystrophy, or limb disabilities struggle with manual control. Existing solutions like joystick-controlled or voice-activated wheelchairs have limitations, including difficulty in usage for individuals with speech impairments or restricted hand mobility.

A **hand gesture-controlled wheelchair** offers an innovative and intuitive solution, allowing users to navigate their environment through simple hand gestures, eliminating the need for complex controls or excessive physical effort.

## Objective
The primary goal of this project is to develop a wheelchair control system that:
- Uses **hand gestures** to navigate the wheelchair in multiple directions.
- Implements **computer vision and machine learning (Mediapipe)** for gesture recognition.
- Establishes **serial communication** between a computer and an Arduino-based system to send movement commands.
- Provides an **accessible, cost-effective, and user-friendly alternative** to traditional wheelchair control systems.

## Hardware Requirements
- **Arduino UNO** (or compatible microcontroller)
- **Webcam** (for real-time hand tracking)
- **Motor Driver Module** (to control wheelchair motors)
- **Battery Pack** (for power supply)
- **Laptop/PC** (for processing gestures)

## Software Requirements
- **Python** (for gesture recognition and communication)
- **OpenCV** (for image processing)
- **Mediapipe** (for hand gesture detection)
- **PySerial** (to communicate with Arduino)
- **Arduino IDE** (for writing and uploading the motor control code)

## How It Works
1. The **webcam** captures the hand gestures of the user.
2. The **Mediapipe library** processes the video feed and detects hand landmarks.
3. The program identifies specific finger positions and determines the intended movement (Forward, Backward, Left, Right, or Stop).
4. Based on detected gestures, the program sends corresponding movement commands to the **Arduino via Serial Communication**.
5. The Arduino processes the received command and controls the **wheelchair motors** accordingly.

## Hand Gesture Commands
| Gesture | Action |
|---------|--------|
| Thumb & Middle Finger Up | Move Forward |
| Thumb & Pinky Finger Up | Turn Left |
| Thumb & Index Finger Up | Turn Right |
| Index & Pinky Finger Up | Move Backward |
| No Fingers Up | Stop |

## Implementation Steps
1. **Set up Arduino and Motor Driver** to control the wheelchair.
2. **Install required Python libraries** (`cv2`, `mediapipe`, `serial` etc.).
3. **Capture webcam input** and process hand landmarks.
4. **Map hand gestures to movement commands** using conditional logic.
5. **Send commands to Arduino via Serial Communication**.
6. **Control wheelchair motors** based on received commands.

## Future Enhancements
- Integration with **IoT** for remote monitoring.
- Implementation of **voice and gesture hybrid control**.
- Use of **AI-based gesture training** for personalized gestures.

## Conclusion
This **Hand Gesture Controlled Wheelchair** provides an intuitive and accessible mobility solution for individuals with disabilities. By leveraging computer vision and embedded systems, this project aims to **enhance independence and improve the quality of life** for users who struggle with traditional control mechanisms.

---



