# ISIC_challenge_2017
Currently over 132,000 melanoma skin cancers occur globally each year,The diagnosis via visual inspection by patients and dermatologists is accurate only about 60 percent of the time.
Moreover, the shortage of dermatologists per capita has abetted the need for computer-aided methods to detect skin cancer.
The [ISIC 2017](https://challenge.isic-archive.com/data) dataset is an aggregation of a large amount of publicly accessible dermoscopy images labeled with ground truth data.

**The ISIC 2017 challenge was divided into 3 tasks:**
* Task 01: Lesion segmentation
* task 02 : Lesion Attribute Detection
* Task 03 : Disease Classification

I worked on Task1 and task3 ,i.e segmentation and classification of images into one of 3 possible classes

# Task 01: Lesion segmentation

For the training I worked with 2000 dermoscopic images and there corresponding Ground-Truth mask from ISIC data set.
For the testing 600 images with the corresponding Ground-Truth
I resized the images to (128,128) for faster processing. 
<img src="seg_img_true.png" width="700">

* Using U_net Model to do the task with Dice coefficient 
 result
 <img src="seg_result.png" width="700">
 <img src="seg_result2.png" width="700">


# Task 03: Disease Classification
For the training I worked with 2000 dermoscopic images and there corresponding Ground-Truth CSV file from ISIC data set.
For the testing 600 images with the corresponding Ground-Truth CSV file.

![GitHub Logo](https://github.com/sif-eddine-boughris/ISIC_challenge_2017/blob/main/ISIC%20chart%20test.png)/
![GitHub Logo](https://github.com/sif-eddine-boughris/ISIC_challenge_2017/blob/main/ISIC%20chart%20train.png)

* Approach
1. Binary classification:
<img src="binar%20class.png" width="700">
2. multi class classification
<img src="multi%20class.png" width="700">
3. multi class classification with Otsu
<img src="binar%20class%20otsu.png" width="700">
4. multi class classification with The true mask
<img src="Binar%20class%20mask.png" width="700">

