This project uses OpenCV, cvzone, and Python to detect free and occupied parking spaces in a parking lot from video or images.

It is divided into two main parts:

Parking Space Picker (ParkingSpacePicker.py)

A tool for selecting and saving parking space coordinates on a parking lot image.

Left-click to add a space, right-click to remove one.

The positions are saved in a file (CarParkPos) using Python’s pickle module.

Parking Detection (main.py)

Loads the saved parking space coordinates from CarParkPos.

Processes the video feed (carPark.mp4) using OpenCV techniques (grayscale, blur, thresholding, dilation).

Detects whether each space is occupied or free based on pixel intensity counts.

Displays a live counter of available parking spaces along with bounding boxes (green = free, red = occupied).

🛠 Tech Stack

Python 

OpenCV – Image and video processing

cvzone – Display text/rectangles on video frames

NumPy – Array operations

Pickle – Save/load parking space positions
