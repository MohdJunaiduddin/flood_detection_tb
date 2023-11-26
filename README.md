# flood_detection_tb
## Dataset
    - 31 images (complete) are in floders like nebraska_20170108t002112
    - images are further divided into images of size 256*256
    - have 4 types of images vv, vh, flood_label and water_body_label
    - the complete image has padding which is empty that empty space can cauze problems while traning so has to deal with it

## Preprocessing
    - built two functions which combine vh and vv image to give a single image 
    - built a function to combine flood_label and water_body_label to only give a image which shows only a flood reigion
    - built a dropper function which drops the image which has significant padding
## modeling
    - found a simple model on stackoverflow for image to image
    - model first down scales and then up scales the image
