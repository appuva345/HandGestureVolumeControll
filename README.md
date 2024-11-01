# HandGestureVolumeControll

This Python script uses OpenCV and MediaPipe to create a hand gesture recognition system that controls system volume based on the distance between the thumb and index finger.

Key Features:
Webcam Feed: The script initializes a webcam feed using OpenCV.

Hand Detection: MediaPipe is used for real-time hand tracking. It detects hand landmarks, specifically the tips of the thumb and index finger.

Volume Control: The distance between the thumb and index finger is measured. This distance is then used to interpolate the system volume:

A shorter distance corresponds to lower volume, while a longer distance corresponds to higher volume.
The volume is controlled through the pycaw library, which interacts with the Windows audio system.
Visual Feedback: The script draws circles around the thumb and index finger and a line connecting them. It also displays a volume bar and percentage on the screen.

Exit Mechanism: The loop continues until the spacebar is pressed, which stops the webcam feed and closes the application.

Use Case:
This program can be used as an intuitive volume control mechanism, allowing users to adjust the audio volume by simply moving their fingers.
