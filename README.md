# Exam Proctoring Project

This project is a real-time proctoring tool using computer vision. It detects and alerts for suspicious behavior during online exams, such as excessive blinking, looking away from the screen, suspicious head turns, and face absence.

## Features
- **Blink Detection:** Counts real blinks and resets every minute. Alerts for excessive blinking (drowsiness).
- **Gaze Detection:** Tracks if the user looks away from the screen. Alerts and beeps if off-screen glances exceed 6 per minute.
- **Head Pose Detection:** Detects significant left/right head turns and displays an on-screen warning.
- **Face Presence Check:** Alerts if no face is detected in the frame.
- **All alerts/messages are displayed on the video frame in real time.**

## Requirements
- Python 3.7+
- OpenCV (`opencv-python`)
- MediaPipe
- NumPy
- Windows OS (for `winsound` beep functionality)

## Installation
1. Clone or download this repository.
2. Install the required packages:
   ```bash
   pip install opencv-python mediapipe numpy
   ```

## Usage
1. Run the `Exam_ProctoringProject.ipynb` notebook (or the script version) in your preferred Python environment.
2. Allow access to your webcam when prompted.
3. The video window will display real-time alerts for:
   - Drowsiness (excessive blinking)
   - Looking away from the screen
   - Suspicious head turns
   - Face not detected
4. Press `Esc` to exit the application.

## Notes
- The project is designed for Windows due to the use of the `winsound` module for beeps. For other OS, replace or remove the beep functionality.
- All alerts are shown on the video frame, not in the terminal.
- For best results, use in a well-lit environment with your face clearly visible to the webcam.

---
<img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/50634f13-32f3-4647-ba88-fe060a891165" />
<img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/0f170a93-6145-4d91-8796-055660381cec" />

