# Abstract

The COVID-19 pandemic has caused many shutdowns in different industries around the world. Sectors such as infrastructure construction and maintenance projects have not been suspended due to their significant effect on people's routine life. In such projects, workers work close together that makes a high risk of infection. The World Health Organization recommends wearing a face mask and practicing physical distancing to mitigate the virus's spread. This project is developed on a computer vision system to automatically detect the violation of face mask wearing and physical distancing among construction workers to assure their safety on infrastructure projects during the pandemic.


# Dataset

A part of the dataset of face masks was obtained from MakeML website that contains 853 images that each image includes one or multiple normal faces with various illumination and poses. The images are already annotated with faces with a mask, without mask, and incorrect mask wearing. To increase the training data 1,000 other images with their annotations were added to the database. The total of 1,853 images was used as the facemask dataset

## Face mask detection Model
		
| Model | Accuracy | 
|--|--|
| Faster R-CNN Inception ResNet V2 | 99.8% |




## Faster R-CNN model

The Faster R-CNN includes the Region Proposal Network (RPN) and the Fast R-CNN as the detector network. The input image is passed through the Convolutional Neural Networks (CNN) Backbone to extract the features. The RPN then suggests bounding boxes that are used in the Region of Interest (ROI) pooling layer to perform pooling on the image's features. Then, the network passes the output of the ROI pooling layer through two Fully Connected (FC) layers to provide the input of a pair of FC layers that one of them determines the class of each object and the other one performs a regression to improve the proposed boundary boxes

## References

[1] Johns Hopkins University, “COVID-19 Map - Johns Hopkins Coronavirus Resource Center,” Johns Hopkins Coronavirus Resource Center, 2020. https://coronavirus.jhu.edu/map.html (accessed Jul. 30, 2020). 

[2] WHO, “Water, sanitation, hygiene and waste management for COVID-19: technical brief, 03 March 2020,” World Health Organization, 2020. 

[3] R. Jahromi, V. Mogharab, H. Jahromi, and A. Avazpour, “Synergistic effects of anionic surfactants on coronavirus (SARS-CoV-2) virucidal efficiency of sanitizing fluids to fight COVID-19,” bioRxiv, p. 2020.05.29.124107, Jun. 2020, doi: 10.1101/2020.05.29.124107. 

[4] R. Ellis, “WHO Changes Stance, Says Public Should Wear Masks,” 2020. https://www.webmd.com/lung/news/20200608/wh o-changes-stance-says-public-should-wear-masks (accessed Jul. 31, 2020). 

[5] S. Feng, C. Shen, N. Xia, W. Song, M. Fan, and B. J. Cowling, “Rational use of face masks in the COVID-19 pandemic,” The Lancet Respiratory Medicine, vol. 8, no. 5. Lancet Publishing Group, pp. 434–436, May 01, 2020, doi: 10.1016/S2213- 2600(20)30134-X.


