Indian number plate detection

Introduction
Number plate recognition is an important application of computer vision used in areas such as traffic monitoring, parking management, and security systems. In this project, we implement a system that detects and recognizes vehicle number plates using a combination of classical image processing techniques and Optical Character Recognition (OCR). Various methods such as edge detection, segmentation, and corner detection are explored to understand how number plates can be localized in an image. A contour-based approach is then used to detect candidate regions, and OCR is applied to extract the plate text. The system demonstrates how traditional computer vision techniques can be used to build a practical solution, while also highlighting their limitations in real-world conditions such as noise, lighting variations, and complex backgrounds.

Correctly detected number plates:- 
     <img width="658" height="316" alt="image" src="https://github.com/user-attachments/assets/f5952c2f-71fd-4607-8bbf-d93242e708e1" />
<img width="672" height="322" alt="image" src="https://github.com/user-attachments/assets/e4ab04e0-5c58-4d45-b992-558e9efb67b6" />
<img width="614" height="311" alt="image" src="https://github.com/user-attachments/assets/fc3ab031-4d5f-4aaf-b465-22aed93c87ed" />

Wrongly detected number plates:-
<img width="640" height="307" alt="image" src="https://github.com/user-attachments/assets/f20fc7f1-463c-42ee-bebd-746e56e52608" />
<img width="642" height="308" alt="image" src="https://github.com/user-attachments/assets/5a41ef76-e207-4a4c-9428-c0f5dc7ab449" />
<img width="576" height="276" alt="image" src="https://github.com/user-attachments/assets/69dcbf7c-961c-43d1-826d-8e1e7a1e51f6" />


    

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
