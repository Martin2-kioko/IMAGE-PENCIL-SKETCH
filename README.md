# IMAGE-PENCIL-SKETCH
# Image Sketch Converter

## Overview
This project utilizes OpenCV to convert a given image into a sketch-like effect. It demonstrates basic image processing techniques, including grayscale conversion, inversion, and Gaussian blurring, to achieve a visually appealing sketch output.

## Requirements
- Python 3.x
- OpenCV library

## Installation
To install the required OpenCV library, run the following command:

```bash
pip install opencv-python

How to Use
Place the image you want to convert in the specified directory (e.g., C:\\Users\\ADMIN\\Desktop\\image.jpg).
Run the script using Python. The script will:
Read the specified image.
Convert the image to grayscale.
Invert the grayscale image.
Apply Gaussian blur to the inverted image.
Invert the blurred image.
Create a sketch effect by dividing the grayscale image by the inverted blurred image.
Save the resulting sketch image to the specified directory (C:\\Users\\ADMIN\\Desktop\\sketch_image.png).
Display the sketch image in a window.
Code Explanation
cv2.imread(): Reads the image from the specified file path.
cv2.cvtColor(): Converts the image from BGR to grayscale.
Inversion: Creates an inverted version of the grayscale image to enhance the sketch effect.
GaussianBlur: Applies a Gaussian blur to the inverted image to smooth out the transitions.
cv2.divide(): Combines the grayscale and inverted blurred images to produce the final sketch effect.
cv2.imwrite(): Saves the sketch image to a specified file path.
cv2.imshow(): Displays the sketch image in a window.
cv2.waitKey(): Waits for a key press to close the displayed image.
cv2.destroyAllWindows(): Closes all OpenCV windows.
