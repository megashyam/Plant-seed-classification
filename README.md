# Plant-seedling-classification

The ability to do so effectively can mean better crop yields and better stewardship of the environment.
The Aarhus University Signal Processing group, in collaboration with University of Southern Denmark, has recently released a dataset containing images of approximately 960 unique plants belonging to 12 species at several growth stages.

The dataset consists of 12 plant species which are:
*Black-grass
*Charlock
*Cleavers
*Common Chickweed
*Common wheat
*Fat Hen
*Loose Silky-bent
*Maize
*Scentless Mayweed
*Shepherds Purse
*Small-flowered Cranesbill
*Sugar beet


## _Preprocessing the images_
Since the leafy area is green and well distinguishable from the background, using a green mask that would sound logical.
For creating mask, which will remove background, we need to convert RGB image to HSV. HSV is alternative of the RGB color model. In HSV, it is easier to represent a color range than in RGB color space.


![alt text](https://codewords.recurse.com/images/six/image-processing-101/hsv.png)


After creating HSV image, we'll create mask based on empirically selected range of green color, convert it to boolean mask and apply it to the origin image.



