# Extract-Text-From-Image
Python will automatically find and extract text from an image.

To extract text content from images using openCV and tesseract.

Prerequisites

To implement this project you should have basic knowledge of:

    Python.
    Tessaract.
    OpenCV.
    Tkinter.
    
Explanation:

    Import all the required libraries (opencv, tkinter, tesseract)
    Provide the location of the tesseract.exe file.
    Tkinter provides GUI functionalities: open an image dialog box so user can upload an image
    Let’s jump to the extract function which takes the path of the image as a parameter
        In this function, we’ll read the image using cv2.imread. We will also resize the image so that we can get well-formatted output for all different sizes of input images.
        Tesseract works on RGB images and opencv reads an image as BGR image, so we need to convert the image and then call tesseract functions on the image. Here,the conversion is done using cv2.cvtCOLOR().
        we have stored height, width, and thickness of the input image using img.shape for later use.
        After the pre-processing, call image_to_data() function of tesseract which returns a string (of extracted text from the image0.
        Print the whole string for better understanding.
        The string is a multiline string, where each line contains extracted text but its first line (starting from zero) contains headings that are not useful for us, so we will skip the very first line.
        Now, split the string to get the extracted text and finally print the extracted text on the screen.    
