# Virtual-Drawing-using-Open-CV
This project implements a virtual drawing application using a webcam and Optical Flow (Lucas-Kanade method) with OpenCV in Python. The program tracks a selected point on the video feed and allows users to draw virtually in the air.

✅ Features
Real-time point tracking using cv2.calcOpticalFlowPyrLK.

Virtual drawing on the camera feed.

Color switching (RGB cycling).

Canvas clear option.

Interactive control via keyboard keys.

 -> How It Works
The program starts by capturing frames from the webcam.

The user clicks on a point in the video window to start tracking.

Lucas-Kanade Optical Flow tracks the movement of the selected point across frames.

A mask is used to draw lines between consecutive tracked points, creating a virtual drawing effect.

The user can:

Press c to change the drawing color.

Press e to erase (clear the canvas).

Press ESC to exit.

⚙️ Requirements
Python 3.x

OpenCV

NumPy

Install dependencies using:
bash
Copy
Edit
pip install opencv-python numpy

-> Controls
Key	Action
Left Click	Select starting point
c	Change color (RGB cycle)
e	Erase/Clear canvas
ESC	Exit program

->  Project Structure
csharp
Copy
Edit

-> Concepts Used
Optical Flow (Lucas-Kanade) for motion tracking.

cv2.calcOpticalFlowPyrLK to compute point movement between frames.

Mask blending with cv2.addWeighted for overlay effect.
Keyboard event handling using cv2.waitKey.
