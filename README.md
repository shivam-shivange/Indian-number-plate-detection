Indian number plate detection

Introduction
Number plate recognition is an important application of computer vision used in areas such as traffic monitoring, parking management, and security systems. In this project, we implement a system that detects and recognizes vehicle number plates using a combination of classical image processing techniques and Optical Character Recognition (OCR). Various methods such as edge detection, segmentation, and corner detection are explored to understand how number plates can be localized in an image. A contour-based approach is then used to detect candidate regions, and OCR is applied to extract the plate text. The system demonstrates how traditional computer vision techniques can be used to build a practical solution, while also highlighting their limitations in real-world conditions such as noise, lighting variations, and complex backgrounds.

Correctly detected number plates:- 
     
Wrongly detected number plates:-

    

Methodology followed :-
•	Dataset is loaded using image and XML annotation files.
•	Images are preprocessed using grayscale conversion and resizing.
•	Noise is reduced using Gaussian blur.
•	Segmentation is applied using thresholding and edge detection.
•	Region growing is used to analyze connected regions.
•	Harris corner detection is used to detect structural points.
•	Edge detection is used to extract contours from images.
•	Contours are filtered based on size and aspect ratio.
•	Candidate plate regions are generated from contours.
•	OCR is applied to each candidate region.
•	Best region is selected based on valid text output.
•	Plate region is cropped and enhanced.
•	OCR extracts final number plate text.
•	Results are displayed with detected plate and text.

Conclusion / Interpretation :
Incorrect detection can occur due to background clutter and similar shapes, which create false edges and confuse contour-based detection. 
Uneven lighting, shadows, and low contrast also affect segmentation and edge detection quality. 
Additionally, tilted or blurred plates distort the shape and weaken features, making detection harder. 
OCR errors can further lead to selecting the wrong region as the number plate.


Code :  https://colab.research.google.com/drive/17ZXLl7K-Jt0pPVzoVOpn3y8Tis49-jvW?usp=sharing
Github : https://github.com/shivam-shivange/Indian-number-plate-detection
