Indian number plate detection

Introduction
Number plate recognition is an important application of computer vision used in areas such as traffic monitoring, parking management, and security systems. In this project, we implement a system that detects and recognizes vehicle number plates using a combination of classical image processing techniques and Optical Character Recognition (OCR). Various methods such as edge detection, segmentation, and corner detection are explored to understand how number plates can be localized in an image. A contour-based approach is then used to detect candidate regions, and OCR is applied to extract the plate text. The system demonstrates how traditional computer vision techniques can be used to build a practical solution, while also highlighting their limitations in real-world conditions such as noise, lighting variations, and complex backgrounds.

Correctly detected number plates:- 
     <img width="658" height="316" alt="image" src="https://github.com/user-attachments/assets/f5952c2f-71fd-4607-8bbf-d93242e708e1" />
<img width="658" height="316" alt="image" src="https://github.com/user-attachments/assets/fbf5f179-996e-4887-9932-96b33ee88670" />
<img width="658" height="316" alt="image" src="https://github.com/user-attachments/assets/24d7b437-053c-4b3a-8619-e27e5a9f3529" />
<img width="658" height="316" alt="image" src="https://github.com/user-attachments/assets/88381a40-12f6-4b0e-9eb8-072fb88ca078" />
<img width="658" height="316" alt="image" src="https://github.com/user-attachments/assets/abcb901b-e4bc-48b9-be01-fad79b50738f" />
<img width="658" height="316" alt="image" src="https://github.com/user-attachments/assets/355b62c3-9e19-4c17-9288-bc7ea5425a1e" />

Wrongly detected number plates:-
<img width="658" height="316" alt="image" src="https://github.com/user-at<img width="658" height="316" alt="image" src="https://github.com/user-attachments/assets/bedf916f-8454-45bf-a304-415adda52f91" />
tachments/assets/6f54c00b-bc01-468c-949d-aeaf18a6a7c4" />
<img width="658" height="316" alt="image" src="https://github.com/user-attachments/assets/a5d97366-9e71-47a3-ac01-9eadb009ee76" />
<img width="658" height="316" alt="image" src="https://github.com/user-attachments/assets/8fa3f37e-dff0-4389-ba6d-a2bbe69114d6" />

    

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
