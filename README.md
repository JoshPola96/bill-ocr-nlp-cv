# Tesseract OCR Image Processing

> **Scope** · MSc coursework (Computer Vision) — published as-is.

> [!NOTE]
> **Built 2021. The ecosystem has moved since.**
> Dependencies here are unpinned, so a clean `pip install` today resolves to
> versions that did not exist when this was written and Tesseract, OpenCV and Pillow have each moved several major versions since. Expect install or
> runtime breakage on a fresh environment. What is on offer is the engineering
> approach and the decisions behind it, not a guaranteed-green build.
> Happy to bring it current if that would be useful — just ask.

This project demonstrates how to use Tesseract OCR for extracting text from images. It processes a set of images of scanned bills and evaluates the accuracy of the OCR results.

## Requirements

- **Python Packages**:
  - `pytesseract`
  - `Pillow`
  - `opencv-python`
  - `glob`
  - `re`
  - `difflib`
  - `numpy`
  
- **System Packages**:
  - `poppler-utils`
  - `tesseract-ocr`
  - `libtesseract-dev`

## Code Overview

1. **Image Processing**:
   - Reads images from specified directories.
   - Applies segmentation to extract regions of interest (ROI).
   - Converts images to grayscale and applies Gaussian blur (for some image types).

2. **Text Extraction**:
   - Uses Tesseract OCR to convert processed images into text.
   - Saves the extracted text into text files.

3. **Accuracy Evaluation**:
   - Compares the extracted text with ground truth files.
   - Calculates and prints the accuracy of the OCR results.

4. **Results**:
   - Displays average accuracy across different image types.

## Notes

- **Pre-Processing**: Segmentation is used to focus on specific areas of the images.
- **Accuracy**: Text extraction accuracy is dependent on image quality and pre-processing techniques.

## Contact

For questions or feedback, please contact:
- **Joshua Peter**: [josh19peter96@gmail.com](mailto:josh19peter96@gmail.com)
