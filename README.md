# Tesseract-Basics

**This repository contains code designed to explore the fundamentals of Tesseract, a robust Optical Character Recognition (OCR) tool. The code in the Jupyter notebook was developed concurrently with the "Python in Digital Humanities" YouTube tutorial, showcasing various Tesseract functionalities as demonstrated in the video.**

## Overview
Optical Character Recognition (OCR) is a transformative technology that converts different types of documents, such as scanned paper documents, PDFs, or digital images, into editable and searchable data. Tesseract is one of the most widely used OCR engines, renowned for its accuracy and versatility.

### Applications of OCR
- **Document Digitization**: Converting printed documents into digital format for efficient storage and retrieval.
- **Automated Data Entry**: Minimizing manual data entry efforts by automatically extracting text from images.
- **Content Searchability**: Enabling search functionality within scanned documents or images.
- **Text Recognition in Natural Scenes**: Extracting text from images captured in natural settings, such as street signs or product labels.

### Significance of Pre-Processing in OCR
Pre-processing is a crucial step in the OCR pipeline to enhance the quality of input images, thereby facilitating the OCR engine's ability to accurately recognize text. Key pre-processing techniques include:

- **Noise Reduction**: Eliminating extraneous noise that can hinder text recognition.
- **Binarization**: Converting images to a binary format to distinguish text from the background.
- **Deskewing**: Correcting any tilt or rotation in the image to properly align the text.
- **Border Removal**: Removing borders that may interfere with text recognition.
- **Morphological Operations (Dilation and Erosion)**: Enhancing text features and eliminating minor imperfections.
- **Color Inversion**: Adjusting the text color from white to black or vice versa, as needed.

Implementing these pre-processing techniques significantly improves the accuracy and reliability of OCR results.

## Libraries Utilized
1. Matplotlib
2. OpenCV
3. PyTesseract
4. Pillow
5. NumPy

## Content
This repository includes all the images utilized and a `.ipynb` file, which encompasses three main sections:

1. **Opening an Image File Using Pillow**
2. **Pre-Processing Techniques in OpenCV**
3. **Final OCR Implementation in Tesseract**

### Pre-Processing Techniques in OpenCV
The pre-processing subsection implements the following techniques:

1. **Opening the Image Using OpenCV and Matplotlib**
2. **Inverting an Image**
3. **Binarization of an Image**
4. **Noise Reduction in an Image**
5. **Morphological Operations (Dilation and Erosion) on an Image**
6. **Deskewing an Image**
7. **Border Removal from an Image**
8. **Adding Borders to an Image**

### Final OCR Implementation in Tesseract
The final OCR subsection examines two types of images:

1. **Image with Latin Text**:
   - This image contains three columns of text. Direct OCR on this image yields suboptimal results as it reads the text left to right. Instead, the text needs to be read column-wise. Various pre-processing techniques were applied to ensure the final OCR output is accurate. The objective was to extract names written in Latin by reading the image column-wise and storing them in a list.

2. **Image with a Footnote**:
   - The task involved extracting the content above a footnote, necessitating the removal of the footnote from the image.

## Credits
- The entire notebook was developed while following the playlist: [Python in Digital Humanities](https://youtube.com/playlist?list=PL2VXyKi-KpYuTAZz__9KVl1jQz74bDG7i&si=aPKzrbkQtgiDwuYu)
- GitHub repository for the tutorial: [OCR Python Textbook](https://github.com/wjbmattingly/ocr_python_textbook)

## Images
All images used or generated through pre-processing techniques and OCR are uploaded in this folder.
<br>
Please note that none of the images used in this project are proprietary. The sources for these images can be found at the following link: [OCR Python Textbook](https://github.com/wjbmattingly/ocr_python_textbook)

## <ins>Note<ins>
The paths used in the file are *Absolute* Paths. You may need to change each path to *Relative* Path. To do this, replace the <ins>/Users/ayaanchoudhury/Desktop/Python Coding/Tesseract<ins> in each path to <ins>/images<ins>
