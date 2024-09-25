
# Driver Drowsiness Detection System with Multi-Tier Alerts

This repository contains a **Driver Drowsiness Detection System** designed to enhance road safety by monitoring the driver’s eyes in real-time using **Raspberry Pi** and a camera. The system provides multi-tier alerts, including sound, light, and SMS notifications, to prevent accidents caused by drowsiness.

## Key Features

### Real-Time Eye Aspect Ratio (EAR) Calculation
- Detects driver drowsiness based on facial landmarks using the EAR method.

### Multi-Tier Notifications
- **Level 1**: Activates a buzzer when initial drowsiness is detected.
- **Level 2**: Turns on a light for persistent drowsiness.
- **Level 3**: Sends an SMS alert after multiple drowsiness alerts.

### LCD Display
- Shows a "Drowsiness Alert!" message when the SMS is sent, which clears after 20 seconds.

### Automatic Timers
- The light turns off after 15 seconds, and the LCD clears after 20 seconds, ensuring seamless operation.

## Hardware Requirements
- Raspberry Pi
- Camera for real-time video capture
- Buzzer for sound alerts
- Light for visual alerts
- 20x4 LCD display for status messages
- GSM module to send SMS alerts

## Libraries Used
- **OpenCV** for image processing
- **dlib** for facial landmark detection
- **RPLCD** for LCD control
- **RPi.GPIO** for Raspberry Pi GPIO control
- **scipy** for EAR calculation

## Setup
1. Clone the repository and install the required Python libraries:
   ```bash
   pip install opencv-python dlib RPLCD RPi.GPIO imutils scipy
   ```
2. Download the `shape_predictor_68_face_landmarks.dat` model and place it in the correct path.
3. Ensure all hardware is connected and configured correctly.
4. Run the program and let the system monitor for drowsiness.

## Motivation
This system aims to prevent accidents caused by driver fatigue by providing early warnings to the driver and nearby passengers. Stay safe on the road and help reduce the risk of accidents!

## Future Improvements
- Integrate with vehicle systems to take corrective actions automatically.
- Implement more sophisticated machine learning models to detect drowsiness with higher accuracy.

---
